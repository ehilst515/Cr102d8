# EF Core & APIs

## What is a Web API?
 - An HTTP service
 - Logic or data accessible over HTTP
 - Used programmatically
 - Accessible across the internet

## Handling HTTP requests with ASP.NET Core
 - The server (kestrel) listens for requests 
 - The middleware pipeline is invoked for each request 
 - Use MVC to route requests to a controller and action
 - Responses flows back down the middleware pipeline

## To create a Web API:

1. Create an ASP.NET Core project

2. Setup MVC 3. Create a class that derives from ControllerBase

4. Implement your action methods

## Attribute routing
 - `[HttpGet/Post/Put/Delete("api/orders")]` 
 - Specify multiple HTTP verbs with AcceptVerbsAttribute
 - Use Route Attribute to specify no HTTP method at all 
 - Controller routes prepended to action routes

 ## Route templates
 - Extract route values (ex "api/orders/{id}")
 - Use route tokens (ex `api/[controller]`) to specify the current controller/action/area
 - Optional route values: {id?}
 - Default route values: {id=latest}
 - Constraints: {id:int}

## Model binding and validation
 - Bind request data to action parameters
 - Bind form data, route values and query string parameters by default 
  - Use [FromBody] to bind the request body using formatters
 - Use [FromRoute/Query/Form/Header] to restrict model binding to a particular source
 - Use data annotations and check `ModelState.isValid`

