This API Gateway works as a middleman to connect between two microservices: [Authentication service 🔑](https://github.com/jerichosiahaya/AuthService) and [Weather service ☁](https://github.com/jerichosiahaya/WeatherService).
If you want to test it, download all three separates repository including this one and then run the web api in local server (recommended using Kestrel).

### How to use the API Gateway?
- Run both microsevices including the gateway
- Go to https://localhost:5021/api/authentication to generate the access token (you will find the username and password hardcoded inside the controller class)
- Copy the access token, then go to https://localhost:5021/api/weather and paste the token in the header request so you can avoid the 401 HTTP Error
- Done, that's all you need to do

This is just a sample for learning purpose. I don't recommend to hardcoded the user identity inside the controller class at all. 

Peace ✌
