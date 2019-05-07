# steps

1. have dockerfile and docker project ready to go (built)
2. gcloud commands

```
gcloud auth login
gcloud config set project MY-GOOGLE-CONSOLE-PROJECT-ID
gcloud builds submit --tag gcr.io/MY-GOOGLE-CONSOLE-PROJECT-ID/quickstart-image .
```

and to configure docker

```
gcloud auth configure-docker
```

3. run to test

```
docker run gcr.io/MY-GOOGLE-CONSOLE-PROJECT-ID/quickstart-image
```
