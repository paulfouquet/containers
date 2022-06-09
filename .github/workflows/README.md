# Build and publish containers

1. Step "Checkout"
   Checks-out your repository under $GITHUB_WORKSPACE, so your workflow can access it.

2. Step "Build containers"
   This step directly uses the docker command to build the docker image under the folder "container/example/" (where the Dockerfile is), tag it with the name "container-example" and add a label containing the GITHUB_RUN_ID which is a unique ID for the GitHub Action workflow run

3. Step "Log in to registry"
   You need to login into the GitHub container registry "ghcr.io"
