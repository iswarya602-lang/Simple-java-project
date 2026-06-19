Dockerfile Explanation
FROM node:18-alpine → Uses the lightweight Node.js 18 image.
WORKDIR /app → Sets /app as the working directory inside the container.
COPY package*.json ./ → Copies package.json and package-lock.json.
RUN npm install → Installs dependencies.
COPY . . → Copies all project files.
EXPOSE 3000 → Opens port 3000.
CMD ["npm", "start"] → Starts the application.
