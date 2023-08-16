# Simple Python Server
## Pushing the image


### Login

```bash
docker login
```

You will be prompted for ID & password

### Push the image

```
docker push [your-dockerhub-id]/simple-http-server
```

### verify

1. Login to Docker Hub
2. Visit https://hub.docker.com/repositories 
3. Notice your image

See how the size of the image is significantly lower

## GCP Container Repository

### Setup & Login

```bash
gcloud components install docker-credential-gcr
docker-credential-gcr configure-docker
docker login asia.gcr.io/staging-data-12358
export DOCKER_HOST="unix://$HOME/.colima/docker.sock"
```

### Check the size of the image

```
docker push asia.gcr.io/staging-data-12358/java-http-server
```

### verify

1. Login to GCP
2. Visit https://console.cloud.google.com/gcr/images/staging-data-12358?project=staging-data-12358
3. Notice your image

See how the size of the image is significantly lower

---

Takeaways & learnings from this exercise :

1. Pushing an Image to registry