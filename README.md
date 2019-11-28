# okta-token-verifier
Example spring boot app to validate an Okta access token
### Setup
Fill in the correct Okta properties in src/main/resources/application.properties and run

`./gradlew bootRun`

### Test your Okta token
```
TOKEN=<your_okta_access_token>
curl -I http://localhost:8080/hello-oauth --header "Authorization: Bearer $TOKEN"
```
If everything went fine this should return 200 OK.
