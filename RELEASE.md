# How to release a new Docker image

Once you're done making adjustments to Dockerfile, a few things need to be done in order to create a new release.

1. Changes must be committed to the repo
2. New git tag and GitHub release must be created
2. Built image must be pushed to Docker Hub

This all can be achieved with two simple scripts. The procedure is following:

1. Build your image with the following command: `sh build.sh`
2. Once it's done, run `sh release.sh`, this will tag your commit and push it to GitHub, and also create a new tag on Docker Hub.