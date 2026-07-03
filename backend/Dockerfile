FROM node:22-alpine
RUN apk add --no-cache openssl libc6-compat
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build
RUN npm run prisma:generate
EXPOSE 4000
# Run db push right before launching the server executable
CMD ["sh", "-c", "npx prisma db push && npm run start:prod"]