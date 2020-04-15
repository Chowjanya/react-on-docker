# react-on-docker
The react app was created by following the [react tutorial](https://reactjs.org/tutorial/tutorial.html).

# To build and tag a name to docker conatiner

docker build -t react-on-docker:dev .

# To run the docker container
docker run     
  -it    
  --rm     
  -v ${PWD}:/app     
  -v /app/node_modules     
  -p 3001:3000     
  -e CHOKIDAR_USEPOLLING=true     
  react-on-docker:dev
  
  The app will be hosted on http://localhost:3001/
