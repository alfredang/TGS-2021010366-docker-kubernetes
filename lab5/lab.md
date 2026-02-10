# Lab 5: Volumes

```bash
# Create a named volume
docker volume create my-data

# List volumes
docker volume ls

# Inspect a volume
docker volume inspect my-data

# Run a container with a named volume mounted
docker run -d -p 5001:5000 --name my-app -v my-data:/app/data lab4

# Write a file to the volume from inside the container
docker exec my-app sh -c "echo 'hello volumes' > /app/data/test.txt"

# Verify the file exists
docker exec my-app cat /app/data/test.txt

# Stop and remove the container
docker stop my-app && docker rm my-app

# Run a NEW container with the same volume — data persists!
docker run -d -p 5001:5000 --name my-app2 -v my-data:/app/data lab4
docker exec my-app2 cat /app/data/test.txt

# Clean up
docker stop my-app2 && docker rm my-app2

# Bind mount: mount current directory into the container
docker run -it -v $(pwd):/app/src lab4 ls /app/src

# Remove a volume
docker volume rm my-data
```
