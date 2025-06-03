# docker-elasticsearch

Custom Elasticsearch Docker image with ICU and Phonetic analysis plugins pre-installed.

## Usage

```
docker pull antistatique/elasticsearch:latest
```

## GitHub Workflow

This repository includes a GitHub Action workflow that can be manually triggered to:
1. Build the Docker image with a specified Elasticsearch version
2. Push the image to Docker Hub as `antistatique/elasticsearch:[version]` and `antistatique/elasticsearch:latest`

### Required Secrets

The following secrets need to be configured in your GitHub repository:
- `DOCKERHUB_USERNAME`: Your Docker Hub username
- `DOCKERHUB_TOKEN`: Your Docker Hub access token

### Running the Workflow

1. Go to the "Actions" tab in your GitHub repository
2. Select the "Build and Push Docker Image" workflow
3. Click "Run workflow"
4. Enter the desired Elasticsearch version (defaults to 8.18.1)
5. Click "Run workflow"
