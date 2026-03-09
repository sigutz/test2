FROM node:20-alpine

WORKDIR /app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy all source files
COPY . .

EXPOSE 5173

# Expose Vite to the Docker network via host configuration
CMD ["npm", "run", "dev", "--", "--host"]
