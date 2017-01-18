# API practice based on the following tutorial
http://idratherbewriting.com/docapis_course_overview/

## APIs
http://www.aerisweather.com/
https://market.mashape.com/fyhao/weather-13

## Calls with cURL

*mashape aqi:*
`curl --get -k --include "https://simple-weather.p.mashape.com/aqi?lat=37.3710062&lng=-122.0375935" -H "X-Mashape-Key: 5cP5gZT72amshYgnshOLzL3WAtzEp1Ap4bajsnPJjJwFWZZzEo" -H "Accept: text/plain"`

result:
```
-H "Accept: text/plain"
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100     2    0     2    0     0      0      0 --:--:--  0:00:04 --:--:--     0HTTP/1.1 200 OK
Content-Type: text/plain
Date: Wed, 18 Jan 2017 02:54:10 GMT
Server: Mashape/5.0.6
Via: 1.1 vegur
X-Powered-By: Express
Content-Length: 2
Connection: keep-alive

63
```

*aeris normals:*
`curl --get -k --include "http://api.aerisapi.com/normals/flagstaff,az?client_id=mAt1HQXREDl8tSFPdkeYp&client_secret=29W59FBZO9sxEj3htznpJhBIm6nVAwUtHhreUzWR&limit=5&filter=hassnow"`

the response has been piped to aeris-normals-response.txt


