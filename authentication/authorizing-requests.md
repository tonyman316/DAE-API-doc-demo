# Authorizing Requests

In most cases, when sending requests to the DaaS services, the request will need to include a header that contains an authorization code.  The authorization code may be acquired by sending a request to DAE’s DaaS token service.  The documentation for the authorization service can be found online here:[ https://enterprise.disasteraware.com/jwt/](https://enterprise.disasteraware.com/jwt/)

To request a new token follow the documentation provided here:[ https://enterprise.disasteraware.com/jwt/\#!/Token/getInitialTokens](https://enterprise.disasteraware.com/jwt/#!/Token/getInitialTokens). 

Please use the provided credentials to complete this request.  The response will include a JSON Web Token \(JWT\) that you will send with the Authorization request header in the following format:.

```text
{
    “Authorization”: “Bearer <insert-json-web-token>”
}
```

  For more information about JWT please visit jwt.io

Login with posting credentials to get access and refresh JSON Web Tokens  


