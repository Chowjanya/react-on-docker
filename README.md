# React App on Docker

The react app was created by following the [react tutorial](https://reactjs.org/tutorial/tutorial.html).

To build: docker build -t react-on-docker .

To run:
docker run     -it     --r    -v ${PWD}:/app     -v /app/node_modules     -p 3001:3000     -e CHOKIDAR_USEPOLLING=true     react-on-docker

