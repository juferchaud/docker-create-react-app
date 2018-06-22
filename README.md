# docker-create-react-app

Run [Facebook Create React App](https://github.com/facebook/create-react-app) in a Node container.

## Run container and run create-react-app
It will execute create-react-app command in `<directory name>` (the directory will be created if needed).
```bash
docker run --rm -v ${PWD}:/usr/src/app/ juferchaud/create-react-app:latest create-react-app <directory name>
```

## Update image in registry
Login && Build && Push
```bash
docker login
docker build -t juferchaud/create-react-app .
docker push juferchaud/create-react-app:latest
```