# Docker Challenge Template

This article introduces and documents the Docker Challenge assignment for the Operating Systems course. These challenges, although basic, cover common scenarios where Docker is used in practice.

The full tutorial is available in the "Docker Challenge Notes (Tutorial).pdf".

## Challenge 1 - Simple Web Server for Static Web

**Folder:** `Challenge1`

1. **Create static files** - Create a `public/index.html` file.
2. **Create a Docker file** - Create a `Dockerfile`.
3. **Create images**
   ```sh
   docker build -t challenge-1 .
   ```
4. **Create the docker container**
   ```sh
   docker create --name challenge-1-container -p 8080:80 challenge-1
   ```
5. **Run the docker container**
   ```sh
   docker start challenge-1-container
   ```
   - Use `docker stop challenge-1-container` to shut down the container.

## Challenge 2 - Creating a Dynamic Application

**Folder:** `Challenge2`

1. **App definition** - Copy `service.js`, `package.json`; Create `Dockerfile`.
2. **Nginx Definition** - Create `nginx.conf`.
3. **Create docker-compose.yml file**
4. **Create an image and run the corresponding docker**
   ```sh
   docker-compose up --build
   ```
   - `docker-compose down` Can shut it down.
