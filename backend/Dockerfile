FROM node:20-alpine

WORKDIR /app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy all source files
COPY . .

# Generate Prisma Client
RUN npx prisma generate

EXPOSE 5000

# Start development server
CMD ["npm", "run", "docker:dev"]
