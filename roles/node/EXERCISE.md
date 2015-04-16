# Candidate Exercise
 
Using your knowlegde of node.js, client side frameworks and using the http://forecast.io API create an application which when accessed via a url can be used to retrieve a weather forecast.

The application should be built with node's HTTP libraries — you may use an abstraction like express. If you scaffold your application using a generator, please document it as such.

You're free to elaborate on the front-end code as much as you like, but we'll be primarily evaluating the back-end aspects.

## How will my submission be reviewed?
 
Your application will be evaluted against the following criteria

| Criteria             | Overview                                                         | 
| -------------------- |:----------------------------------------------------------------:| 
| **Test Coverage**    | How well tested is your code, (**We will run your test suite**)  |
| **Code Quality**     | Code is well structured, readable and documented. Source is tidy |
| **Configurability**  | Can aspects of your application be configured                    |
| **Modularity**       | Can parts of your application be reused                          |
| **Durability**       | How resilient is your application to known and unexpected errors |

## Scenarios

The items below should be considered to be applicable to all scenarios.

- **Support both basic HTML and JSON responses**
- **Unit & Functional test suites**
 
### Scenario One: Display a weather forecast by location
 
A weather forcast should be displayed based upon the location specified in the url.
A location might be a state or territory, municipal locality, or city name.
For the purposes of the test it will be alphanumeric.
 
- Expected URL: http://localhost:<port>/weather/:location
- Example  URL: http://localhost:<port>/weather/( sydney | brisbane )
 
### Scenario Two: Display a weather forecast by location filtered by day
 
A weather forcast should be displayed based upon the location and day specified in the url.
The application is not expected to be timezone aware. The weekday is always in the future
(for example—if the current day is Wednesday and the requested time is Tuesday, the weather
returned should be for *next* Tuesday. If the requested day is the same as the current day,
the weather returned should be for one week from the current day.)
 
- **Expected URL:** http://localhost:\<port\>/weather/:location/:weekday
- **Example  URL:** http://localhost:3000/weather/vladivostok/tuesday
 
### Scenario Three: Display a weather forecast for today
 
A weather forcast should be displayed based upon the location and the current day.
 
- **Expected URL:** http://localhost:\<port\>/weather/:location/today
- **Example  URL:** http://localhost:\<port\>/weather/sydney/today
 
#### Supporting Material:
 
- API: https://developer.forecast.io/
