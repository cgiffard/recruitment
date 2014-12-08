# Candidate Exercise
 
Using your knowlegde of node.js, client side frameworks and using the http://forecast.io API create an application which when accessed via a url can be used to retrieve a weather forecast.

## How will my submission be reviewed?
 
Your application will be evaluted against the following criteria

| Criteria             | Overview                                                         | 
| -------------------- |:----------------------------------------------------------------:| 
| **Test Coverage**    | How well tested is your code, ( **We will run your test suite** )|
| **Code Quality**     | Code is well structured, readable and documented. Source is tidy |
| **Configurability**  | Can aspects of your application be configured                    |
| **Modularity**       | Can parts of your application be reused                          |
| **Durability**       | How resilient is your application to known and unexpected errors |

## Scenarios

The items below should be considered to be applicable to all scenarios.

- **Support both basic HTML and JSON responses**
- **UNIT & Functional test suites**
 
### Scenario One: Display a weather forecast by location
 
A weather forcast should be displayed based upon the location specified in the url.
 
- Expected URL: http://localhost:<port>/weather/:location
- Example  URL: http://localhost:<port>/weather/( sydney | brisbane )
 
### Scenario Two: Display a weather forecast by location filtered by day
 
A weather forcast should be displayed based upon the location and day specified in the url.
 
- **Expected URL:** http://localhost:\<port\>/weather/:location/:weekday
- **Example  URL:** http://localhost:\<port\>/weather/:location/( monday | tuesday | etc .. )
 
### Scenario Three: Display a weather forecast for today
 
A weather forcast should be displayed based upon the location and the current day.
 
- **Expected URL:** http://localhost:\<port\>/weather/:location/today
- **Example  URL:** http://localhost:\<port\>/weather/sydney/today
 
#### Supporting Material:
 
- API: https://developer.forecast.io/
