from node:20-alpine

workdir /app

copy package*.json ./

run npm ci

copy . ./

run npm run build

env api_url=http://localhost:3000

cmd ["npx", "vite", "preview", "--host", "0.0.0.0", "--port", "3000"]