FROM node:18-alpine
WORKDIR /app
COPY ./api/package*.json ./
RUN npm ci --only=production
COPY ./api/ ./
EXPOSE 5000
CMD ["npm", "start"]