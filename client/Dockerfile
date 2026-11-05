
FROM node:20-alpine

WORKDIR /app

COPY package*.json ./

# Disable Cypress binary download
ENV CYPRESS_INSTALL_BINARY=0

# Install project dependencies
RUN npm install

COPY . .

EXPOSE 5173

CMD ["npm", "run", "dev", "--", "--host", "0.0.0.0"]

