# CONTRIBUTING

## How to run the Dockerfile locally

```
docker build -t IMAGE_NAME .
docker run -dp 5000:5000 -w /app -v "$(pwd):/app" IMAGE_NAME sh -c "flask run --host 0.0.0.0"

e.g.:
docker build -t flask-smorest-api .
docker run -dp 5000:5000 -w /app -v "$(pwd):/app" flask-smorest-api
```
