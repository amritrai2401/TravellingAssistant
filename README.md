https://user-images.githubusercontent.com/86003701/138207641-b6294191-4166-497e-bf50-d1f5a052fee0.mp4

Used React app for making frontend/Client.

Used 5 Api(google maps,google places,open weather map, geolocation, travel advisor) for fetching data.

The website provides-:

• Data(mobno,ratings,price,etc) about hotels, restaurants,tourist attractions and u can filter it by ratings.

• Link to tripadvisor.in for reviews and more info about a particular restaurants & hotels.

• Weather condition by on map.

• Link of the website of the particular restaurant and hotel, if they have.


# More details-:
Used 5 api for making this amazing in following ways💛💛.
* Used Google maps api for having the google map in our app.
* Used Google places api for 1)having search recommendation while typing  2)having latitude and longitude of the place if its in google data.
* Used built in Geolocation api for getting user's current latitude and longitude.
* Used Travel Advisor api's 3 endpoints for having 1)hotel details in boundries defined,2)restaurants details in boundries defined and 3)attraction details in boundries defined. The detail includes image,pricing,website link,phone,rating,certification,link to website reviews in tripadvisor and all other stuff,if present.
* Used Open Weather Map api for getting weather data in the boundry defined , if present🎊


Whenever we select any category like hotels,rating above 4.5 etc, we pass the that category things in a collection which is then passed to Google maps component as collection.map(with latitude & longitude of items)(.map is used for external things to be shown on google maps).✨

Used MaterialUi for icons,searchbox styling,circular progress(loading) component.💛


Used useState for managing state,i.e, like numbers(boundry changes,lat/longitude changes,loading component) when they will increase/decerease etc.

Used useState for managing bool(loading component) when they will set to true/false.

Used useEffect,so that whenver user changes map either by searching,allowing to use location or manually by scrolling, Travel advisor & weather api requests data for the new boundries. When This useeffect starts,we set the loading = true and when all data restaurant,hotel etc data is fetched we set the loading = false and return the data.

Data is returned in json format from server.

Whenever user searches,allows its location to be used(instead of manually moving the map) a place it gets only latitude & longitude of a particular point, so I mantained the boundries of map [50,50,50,50] units away from the central point user got when searched.💙💙
