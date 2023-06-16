# Machine Learning API on Cloud Build

### 1. Write the Flask server app using Python
Save the model in '.h5' format in the same directory as main.py
Load the model and write Flask code in main.py
Test the Flask server locally by running main.py, copy the assigned local URL to test.py then run it with test images.
### 2. Setup On Google Cloud
Enable Cloud Run and Cloud Build API
### 3. Install Google Cloud SDK
https://cloud.google.com/sdk/docs/install
### 4. Dockerfile, requirements.txt, .dockerignore
https://cloud.google.com/run/docs/quickstarts/build-and-deploy#containerizing
### 5. Cloud build & deploy
```
gcloud builds submit --tag gcr.io/rice-hero-389314/index
```
```

gcloud run deploy --image gcr.io/rice-hero-389314/index --platform managed
```

### Test
You can test local with postman before deploy it to the cloud run. and you also can test it in postman again after you deploy to cloud run
