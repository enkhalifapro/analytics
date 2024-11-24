# Build Instructions
- Build Docker Image ```$ docker build -t coworking .```
- Local docker run ```$ docker run coworking -d -p 5153:5153```

# Deploy
- Every commit to main branch triggers codebuild pipeline which runs the following steps:
  - Build Docker image.
  - Push docker image to ECR repository. 