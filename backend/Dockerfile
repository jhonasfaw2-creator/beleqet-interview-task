
FROM node:22-alpine
RUN apk add --no-cache openssl libc6-compat
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build
RUN npm run prisma:generate
EXPOSE 4000
# Update this line to push the database schema before launching the production server
CMD ["sh", "-c", "npx prisma db push && npm run start:prod"]