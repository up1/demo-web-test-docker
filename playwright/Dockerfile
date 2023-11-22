FROM mcr.microsoft.com/playwright:v1.40.0-jammy
WORKDIR /app
COPY package.json package.json
RUN --mount=type=cache,target=/root/.npm npm install
COPY . .
CMD ["npm", "run", "test"]