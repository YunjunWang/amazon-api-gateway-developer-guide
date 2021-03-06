# Initialize API Setup in API Gateway<a name="create-api-resources-methods"></a>

 For this example, we use a simplified [PetStore](http://petstore-demo-endpoint.execute-api.com/petstore/pets) API, with the HTTP integration, that exposes the `GET /pets` and `GET /pets/{petId}` methods\. The methods are integrated with the two HTTP endpoints, respectively, of `http://petstore-demo-endpoint.execute-api.com/petstore/pets` and `http://petstore-demo-endpoint.execute-api.com/petstore/pets/{petId}`\. The API handles `200 OK` responses\. The examples focus on the essential programming tasks for creating an API in API Gateway, taking advantage of default settings when possible\. 

 Because of the default settings, the resulting API is edge\-optimized\. An alternative is to [set up a regional API](create-regional-api.md)\. To set up a regional API, you must set explicitly the endpoint type of the API as `REGIONAL`\. To set up an edge\-optimized API explicitly, you can set `EDGE` as the type of the `endpointConfiguration`\.

 When setting up an API, you must choose a region\. When deployed, the API is region\-specific\. For an edge\-optimized API, the base URL is of the `http[s]://{restapi-id}.execute-api.amazonaws.com/stage` format, where `restapi-id}` is the API's [id](http://docs.aws.amazon.com/apigateway/api-reference/resource/rest-api/#id) value generated by API Gateway\. You can assign a custom domain name \(for example, `apis.example.com`\) as the API's host name and call the API with a base URL of the `https://apis.example.com/myApi` format\. 

**Topics**
+ [Set up an API Using the API Gateway Console](create-api-using-console.md)
+ [Set up an Edge\-Optimized API Using AWS CLI Commands](create-api-using-awscli.md)
+ [Set up an Edge\-Optimized API Using the AWS SDK for Node\.js](create-api-using-awssdk.md)
+ [Set up an Edge\-Optimized API Using the API Gateway REST API](create-api-using-restapi.md)
+ [Set up an Edge\-Optimized API by Importing Swagger Definitions](create-api-using-swagger.md)
+ [Set up a Regional API in API Gateway](create-regional-api.md)