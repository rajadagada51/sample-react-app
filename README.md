# sample-react-app 

In order to start the user interface from local machine , clone this repository and run the following commands

```
cd sample-react-app
npm i
npm start
```

Production Build. This will produce static html/css files and deploy these onto the any webserver, like Nginx
```
npm run build
```

Below are the instructions for the K8s deployment

1. Build the docker image
2. Push the Docker image either to ACR or JFfrog registries
3. Create a secret in namespace to authenticate repositoris.
4. Update acr registry/imagename:tag and registry secret in the Deployment YAML file.

Other option: AKS can authenticate ACR without password using the SP or MI.


