# AWS WEB APP

This repo is using CloudFormation to Depoly the infrastucture as seen below in the architecture diagram.
![The Architecture Diagram](./AWSWebApp.jpeg)

### Creating the Network Stack
```
cd AWSWebApp
./create.sh AWSWEBAPP-Network network.yml network-parameters.json aws-user-profile
```

### Updating the Network Stack
```
cd AWSWebApp
./update.sh AWSWEBAPP-Network network.yml network-parameters.json aws-user-profile
```
## The server stack is cross-referencing values from the Network stack e.g VPCID
### Creating the Server Stack
```
cd AWSWebApp
./create.sh AWSWEBAPP-Servers servers.yml server-parameters.json aws-user-profile
```

### Updating the Server Stack
```
cd AWSWebApp
./update.sh AWSWEBAPP-Servers servers.yml server-parameters.json aws-user-profile
```