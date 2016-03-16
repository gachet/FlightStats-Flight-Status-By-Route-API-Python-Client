# FlightStats-Flight-Status-By-Route-API-Python-Client
Provides an FlightStats.com FlightStatus By Route Client written in Python.

## Usage
Before starting, you must obtain an account with FlightStats.com.

```Python
from flightstats_api_client.api_client import FlightStatusByRouteAPIClient

app_id = 'Your FlightStats.com API app_id'
app_key = 'Your FlightStats.com API app_key'
client = FlightStatusByRouteAPIClient(app_id, app_key)

departure_airport_code = 'SEA'
arrival_airport_code = 'ORD'
departure_date = '2016-12-19' # Must be in yyyy-mm-dd format

response = client.get_flights_by_departure_date(departure_airport_code,
                                                arrival_airport_code,
                                                departure_date)
```
