from node:20-alpine

copy . ./

run npm install

env port=3000

env database_url=postgres://taskflow:taskflow@localhost:5432/taskflow

env app_env=local

env app_version=dev

cmd ["npm", "run", "dev"]