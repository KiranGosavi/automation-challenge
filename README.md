Docker commands to build the custom nginx webserver image:

```
#docker-compose up -d --build

#docker-compose ps

     Name         Command   State          Ports        
--------------------------------------------------------
nginx-webserver   nginx     Up      0.0.0.0:5000->80/tcp

```

Your static page should be accessible at http://localhost:5001/

To clean up your resources and stop docker container us below command:

```
#docker-compose down

```

##TODO##

- Create kubernetes cluster deployment with this custom image
- Make the webserver  accessible on http://automation-challange.cgi.com in the browser
- Add HTTPS only access
- Add TLS certificate
- CI/CD pipeline