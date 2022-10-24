npx create-react-app frontend
docker build -f Dockerfile.dev .
docker images
docker run -it -p 3000:3000 <imageId>
docker-compose up



If you are using any version of Windows and your React app is not automatically reloading after a code change, you can add this environment variable to your compose file:

services:
  web:
    environment:
      - CHOKIDAR_USEPOLLING=true     # NOT WORKING