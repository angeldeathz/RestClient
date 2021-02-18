# Restclient
_This is a simple Library that makes REST Request to any API Rest._

## Why RestClient?
_This Library uses the HttpClient dotnet class and this library abstracts the usage of HttpClient.
So, the usage is simplest._

# Compatibility
This Library is compatible with just NET 5.0, but, soon will be availible for dotnet core 3.1 and
.NET Framework.

# About the Creator
Hi I'm David and I'm a IT Engineer and .NET Developer,
I'm From Chile and actually I'm working like FullStack Developer ;)
I like create code, help another people to build simplest and beauty code.

# Usage
var client = new RestClient(); <br/>
var response = await client.GetAsync<THE_CLASS_TO_DESERIALIZE>(YOUR_URL);

How you can see, you can pass some class to deserialize the response.

RestClient was made for async/await usage, but you can use it for synchronous operations easily, for Example:

var client = new RestClient();<br/>
var response = client.GetAsync<THE_CLASS_TO_DESERIALIZE>(YOUR_URL).Result;<br/>
