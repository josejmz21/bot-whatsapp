FROM node:18-bullseye as bot
WORKDIR /app
# Install pnpm
RUN npm install -g pnpm
COPY package*.json ./
RUN npm i
COPY . .
ARG RAILWAY_STATIC_URL
ARG PUBLIC_URL
ARG PORT
CMD ["npm", "start"]
