FROM node:16-alpine

WORKDIR /app

COPY package*.json ./

# Install only production dependencies
RUN npm install --omit=dev

COPY . .

# Expose backend port
EXPOSE 3500

CMD ["node", "index.js"]
