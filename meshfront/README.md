Building a frontend container for mesh access:

docker build -t yourname/meshfront:v1 -f Dockerfile .
docker push yourname/meshfront:v1
docker run -d --name meshfront -p 5005:5005 yourname/meshfront:v1