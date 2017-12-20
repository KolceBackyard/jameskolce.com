# The Brain of James Kolce

## 1. Build the Docker image

```
docker build -t jameskolce/brain .
```

## 2. Run the Docker image for development

This will mount the source code inside the container, so you can work while it’s running.

```
docker run --env NODE_ENV=development --name jameskolce/brain -v (pwd)/src:/var/lib/ghost/content/themes/brain -p 2368:2368 -d brain
```
