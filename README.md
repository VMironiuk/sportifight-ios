# Simple sport prediction app for iOS.

# API

## Base URL

`Base URL` - TBD

# Model specs

## Country by ID

### Country
| Property     | Type       |
|--------------|------------|
| `id`         | `Int`      |
| `name`       | `String`   |
| `alpha2code` | `String`   |
| `alpha3code` | `String`   |
| `capital`    | `String`   |
| `flag`       | `String`   |
| `region`     | `String`   |
| `subregion`  | `String`   |
| `timezones`  | `[String]` |

### Payload contract
```
GET /api/v1/countries/:id

200 RESPONSE

{
    "data": [
        {
            "id": 5,
            "name": "Argentina",
            "alpha2code": "AR",
            "alpha3code": "ARG",
            "capital": "Buenos Aires",
            "flag": "https://cdn.elenasport.io/flags/svg/5",
            "region": "Americas",
            "subregion": "South America",
            "timezones": [
                "UTC-03:00"
            ]
        }
    ]
}
```

## All Countries

### Countries
TBD

### Payload contract 
```
GET /api/v1/countries

200 RESPONSE

{
    "data": [
        {
            "id": 1,
            "name": "Albania",
            "alpha2code": "AL",
            "alpha3code": "ALB",
            "capital": "Tirana",
            "flag": "https://cdn.elenasport.io/flags/svg/1",
            "region": "Europe",
            "subregion": "Southern Europe",
            "timezones": [
                "UTC+01:00"
            ]
        },
        {
            "id": 3,
            "name": "Algeria",
            "alpha2code": "DZ",
            "alpha3code": "DZA",
            "capital": "Algiers",
            "flag": "https://cdn.elenasport.io/flags/svg/3",
            "region": "Africa",
            "subregion": "Northern Africa",
            "timezones": [
                "UTC+01:00"
            ]
        },
        {
            "id": 5,
            "name": "Argentina",
            "alpha2code": "AR",
            "alpha3code": "ARG",
            "capital": "Buenos Aires",
            "flag": "https://cdn.elenasport.io/flags/svg/5",
            "region": "Americas",
            "subregion": "South America",
            "timezones": [
                "UTC-03:00"
            ]
        },
        . . .
}
```

