# ml-service
---
ML Service and REST API with Django

###Run local server
```
docker-compose build
docker-compose up -d
```

###List of available API Endpoints
```
http://127.0.0.1:8000/api/v1
```

###Prediction
```
POST http://127.0.0.1:8000/api/v1/income_classifier/predict
```
#####Body
```
{
    "age": 37,
    "workclass": "Private",
    "fnlwgt": 34146,
    "education": "HS-grad",
    "education-num": 9,
    "marital-status": "Married-civ-spouse",
    "occupation": "Craft-repair",
    "relationship": "Husband",
    "race": "White",
    "sex": "Male",
    "capital-gain": 0,
    "capital-loss": 0,
    "hours-per-week": 68,
    "native-country": "United-States"
}
```