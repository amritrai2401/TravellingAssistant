Used 5 api for making this amazing app💛💛.
* Used Google maps api for having the google map in our app.
* Used Google places api for 1)having search recommendation while typing  2)having latitude and longitude of the place selected from recommendation.
* Used built in Geolocation api for getting user's current latitude and longitude.
* Used Travel Advisor api's 3 endpoints for having 1)hotel details in boundries defined,2)restaurants details in boundries defined and 3)attraction details in boundries defined. The detail includes image,pricing,website,phone,rating,certification and all other stuff,if present.
* Used Open Weather Map api for getting weather data in the boundry defined , if present.


Whenever we select any category like hotels,rating above 4.5 etc, we pass the that category things in a collection which is then passed to Google maps component as collection.map(with latitude & longitude of items)(.map is used for external things to be shown on google maps).


Used useState for managing boundry changes,lat/longitude changes etc.

Used useEffect,so that whenver user changes map either by searching,allowing to use location or manually by scrolling, Travel advisor & weather api requests data for the new boundries.

Whenever user searches,allows its location to be used(instead of manually moving the map) a place it gets only latitude & longitude of a particular point, so I mantained the boundries of map [50,50,50,50] units away from the central point user got when searched.
