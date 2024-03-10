ARG BUILD_FROM
FROM ${BUILD_FROM}

# Set workdir
WORKDIR /app

# Copy root filesystem
COPY app.js /app
COPY package.json /app
COPY package-lock.json /app

# Run
RUN npm ci
COPY . /app

CMD ["npm", "start"]
