[//]: # (Basic docu)

`{
 "date": "2015-09-01",
 "description": "sunny",
 "maxTemp": 22,
 "minTemp": 20,
 "windSpeed": 12,
 "danger": false
}`

Represents a day's forecast.

| Element | Description | Type | Notes |
| ---- | ---- | ---- | ---- |
| date | Date of the forecast | string | Format is YYYY-MM-DD |
| description | Text description of the weather | string | Valid Values: "sunny", "overcast", "partly cloudy", "raining", or "snowing" |
| maxTemp | Hight temperature | number | Degrees Celsius |
| minTemp | Low temperature | number | Degrees Celsius |
| winSpeed | Wind Speed | number | Kilometers per hour |
| danger | True if the weather conditions are dangerous; otherwise, false | boolean |  |

[//]: # (Complex docu)

`{
 "longitude": 47.60,
 "latitude": 122.33,
 "forecasts": [
 {
 "date": "2015-09-01",
 "description": "sunny",
 "maxTemp": 22,
 "minTemp": 20,
 "windSpeed": 12,
 "danger": false
 },
 {
 "date": "2015-09-02",
 "description": "overcast",
 "maxTemp": 21,
 "minTemp": 17,
 "windSpeed": 15,
 "danger": false
 },
 {
 "date": "2015-09-03",
 "description": "raining",
 "maxTemp": 20,
 "minTemp": 18,
 "windSpeed": 13,
 "danger": false
 }
 ]
}`

Represents 3 days forecast

| Element | Description | Type | Notes |
| ---- | ---- | ---- | ---- |
| longitude | longitude of place weather data | number | Degrees |
| latitude | latitude of place weather data | number | Degrees |
| forecast | Daily forecast | arrays of objects | List of 3 days forecast |
| &nbsp; &nbsp;date | Date of the forecast | string | Format is YYYY-MM-DD |
| &nbsp; &nbsp;description | Text description of the weather | string | Valid Values: "sunny", "overcast", "partly cloudy", "raining", or "snowing" |
| &nbsp; &nbsp;maxTemp | Hight temperature | number | Degrees Celsius |
| &nbsp; &nbsp;minTemp | Low temperature | number | Degrees Celsius |
| &nbsp; &nbsp;winSpeed | Wind Speed | number | Kilometers per hour |
| &nbsp; &nbsp;danger | True if the weather conditions are dangerous; otherwise, false | boolean |  |


[//]: # (Basic docu)

`{
 "meeting" : {
 "time": "2015-09-01 10:00",
 "duration": 60,
 "description": "2016 Strategic Planning Meeting",
 "location": "Building 23, Room 206",
 "reminder": 15,
 "invitees": ["michael@example.com", "thelma@example.com",
 "david@example.com", "leon@example.com"]
 }
}`

Represents a request to create a meeting

| Element | Description | Type | Require | Notes |
| ---- | ---- | ---- | ---- | ---- |
| meeting | Top level | object | required |  |
| &nbsp; &nbsp; time |  time that the comment was post | string | required | YYYY-MM-DD HH:MM:SS Greenwich Mean Time |
| &nbsp; &nbsp; duration |  Meeting duration | number | required | Minutes. Default 30 min |
| &nbsp; &nbsp; description |  Meeting description | string | required |  |
| &nbsp; &nbsp; location |  Meeting location/adress | string | optional | Default empty string |
| &nbsp; &nbsp; reminder |  Meeting reminder | number | optional | Minutes. Default 10 min |
| &nbsp; &nbsp; invitees |  Meeting participants | array of strings | optional | default empty array |






