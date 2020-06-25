# For Develop

Use following cmd to bind project `themes/custom` with Keycloak docker

```
docker run -d -p 9000:8080 -e KEYCLOAK_USER=admin -e KEYCLOAK_PASSWORD=admin --mount type=bind,source=/path/to/themes/custom,target=/opt/jboss/keycloak/themes/custom quay.io/keycloak/keycloak:10.0.2
```
