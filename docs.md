Submit a PDF document as proof of completion into the OTOT Task A1 assignment on Canvas. The document should contain the following information:  
a. Student Name and Matriculation Number  
Daniel Tan Ren Jie  
A0199712U  
b. Link to GitHub repository  
https://github.com/cookiedan42/OTOT-A1  
c. Instructions on how to run the Docker container  
  
a1  


to dockerize
docker-compose 
map app folder over to container
    index.js and public folder with the required files
create volume for node_modules

dockerfile
setup node in the container through an image
copy over packages.json
install required packages in container
(.dockerignore is set up to ignore node_modules folder)

running
navigate into app folder
`docker compose up --build` in command line to launch and force rebuild  
connect to `localhost:3000` in web browser  
  
a2  
dockerizing

docker compose based off nginx image
map outer_access:inner80
map folder containing index.html to html folder in container

running
navigate into nginx-sample folder
`docker compose up --build` in command line to launch and force rebuild  
connect to `localhost:3001` in web browser  


a3
dockerize
combine the two docker-compose services
- remap the folders to match their new relative location
- give a new port mapping for the two services

running
navigate into nginx-sample folder
`docker compose up --build` in command line to launch and force rebuild  
connect to `localhost:8001` in web browser for app  
connect to `localhost:8002` in web browser for nginx-sample

d. Screenshot proofs of localhost showing the webpage (note that A1.1 and A1.2 will show different webpage)  
e. Any other relevant information you wish to provide for the marking team  