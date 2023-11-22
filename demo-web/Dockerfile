FROM node:18-alpine3.17 AS step_01
WORKDIR /app
COPY package.json .
RUN npm install
COPY . .
RUN npm run build

FROM nginx:1.25.3-alpine
COPY --from=step_01 /app/dist/ /usr/share/nginx/html/