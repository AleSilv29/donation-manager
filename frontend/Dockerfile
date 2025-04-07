# Build Angular app
FROM node:18 as build
WORKDIR /app
COPY . .
RUN npm install
RUN npm run build

# Serve with Nginx
FROM nginx:alpine
COPY --from=build /app/dist/first /usr/share/nginx/html
COPY nginx.conf /etc/nginx/conf.d/default.conf
