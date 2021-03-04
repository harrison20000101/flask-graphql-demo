# Build and Run
## Build the image
docker build -t flask-web:latest .

## Run the container
docker run -d -p 5000:5000 flask-web
