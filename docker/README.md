##Build image 

docker build -t terdiaphp/app:latest -f docker/app/Dockerfile docker/app

##Run Container 

docker run --rm -it -p 8080:80 -v $(pwd)/application:/var/www/html/public terdiaphp/app:latest