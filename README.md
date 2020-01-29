# Simple Helm chart to deploy a Microservice app in Kubernetes
I use this chart to test my deployment of microservices apps in kubernetes
# How to use
- helm install --name server --set name=sayhello --set image.repository=jonathanlareau/spring-boot-java-http-server --set service.port=3000 .
- helm install --name client --set name=api --set image.repository=jonathanlareau/spring-boot-java-http-client --set service.port=8080 .
- helm install --name angular --set name=angular --set image.repository=jonathanlareau/simple-angular-hello --set service.port=4200 .

