# ML_repository
Creating a Repository template for ML applications fulfilling SQA requirements 

## Overview
Creating a Repository template for ML applications fulfilling SQA requirements 

## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites
What things you need to install the software
- Python 3.5.2+

### Installing
To run the server, please execute the following from the root directory:

```
pip3 install -r requirements.txt
python3 -m openapi_server
```

and open your browser to here:

```
http://localhost:8080/api/v1/ui/
```

Your OpenAPI definition lives here:

```
http://localhost:8080/api/v1/openapi.json
```

## Running the tests
To launch the integration tests, use pytest:
```
sudo pip install -r test-requirements.txt
pytest
```

## Built With

* [EGI Container Compute](https://www.egi.eu/services/cloud-container/)
* [EGI DataHub](https://www.egi.eu/services/datahub/)
* [EGI Check-In](https://www.egi.eu/services/check-in/)

## Contributing

Please read [CONTRIBUTING.md](
https://github.com/pcalatayud-prog/ML_repository/blob/main/CODE_OF_CONDUCT.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

For the versions available, see the [tags on this repository](https://github.com/ML_repository/issues/labels). 

## Authors


* **Pablo Calatayud**

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Prevent file overriding

After first generation, add edited files to _.openapi-generator-ignore_ to prevent generator to overwrite them. Typically:
```
server/controllers/*
test/*
*.txt
```
