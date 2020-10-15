# wazo-applicationd-client
Applicationd

This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: 0.1.0
- Package version: 1.0.0
- Build package: org.openapitools.codegen.languages.PythonClientCodegen

## Requirements.

Python 2.7 and 3.4+

## Installation & Usage
### pip install

If the python package is hosted on a repository, you can install directly using:

```sh
pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
```
(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)

Then import the package:
```python
import wazo_applicationd_client
```

### Setuptools

Install via [Setuptools](http://pypi.python.org/pypi/setuptools).

```sh
python setup.py install --user
```
(or `sudo python setup.py install` to install the package for all users)

Then import the package:
```python
import wazo_applicationd_client
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```python
from __future__ import print_function

import time
import wazo_applicationd_client
from wazo_applicationd_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = wazo_applicationd_client.Configuration(
    host = "http://localhost"
)



# Enter a context with an instance of the API client
with wazo_applicationd_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = wazo_applicationd_client.ApplicationApi(api_client)
    application_uuid = 'application_uuid_example' # str | 
call_id = 'call_id_example' # str | 

    try:
        # Call Answer
        api_response = api_instance.call_answer10_applications_application_uuid_calls_call_id_answer_put(application_uuid, call_id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ApplicationApi->call_answer10_applications_application_uuid_calls_call_id_answer_put: %s\n" % e)
    
```

## Documentation for API Endpoints

All URIs are relative to *http://localhost*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*ApplicationApi* | [**call_answer10_applications_application_uuid_calls_call_id_answer_put**](docs/ApplicationApi.md#call_answer10_applications_application_uuid_calls_call_id_answer_put) | **PUT** /1.0/applications/{application_uuid}/calls/{call_id}/answer | Call Answer
*ApplicationApi* | [**call_hangup10_applications_application_uuid_calls_call_id_delete**](docs/ApplicationApi.md#call_hangup10_applications_application_uuid_calls_call_id_delete) | **DELETE** /1.0/applications/{application_uuid}/calls/{call_id} | Call Hangup
*ApplicationApi* | [**call_mute_start10_applications_application_uuid_calls_call_id_mute_start_post**](docs/ApplicationApi.md#call_mute_start10_applications_application_uuid_calls_call_id_mute_start_post) | **POST** /1.0/applications/{application_uuid}/calls/{call_id}/mute/start | Call Mute Start
*ApplicationApi* | [**call_mute_stop10_applications_application_uuid_calls_call_id_mute_stop_post**](docs/ApplicationApi.md#call_mute_stop10_applications_application_uuid_calls_call_id_mute_stop_post) | **POST** /1.0/applications/{application_uuid}/calls/{call_id}/mute/stop | Call Mute Stop
*ApplicationApi* | [**create_node_with_calls10_applications_application_uuid_nodes_node_name_post**](docs/ApplicationApi.md#create_node_with_calls10_applications_application_uuid_nodes_node_name_post) | **POST** /1.0/applications/{application_uuid}/nodes/{node_name} | Create Node With Calls
*ApplicationApi* | [**register_application10_applications_application_name_post**](docs/ApplicationApi.md#register_application10_applications_application_name_post) | **POST** /1.0/applications/{application_name} | Register Application
*StatusApi* | [**status_status_get**](docs/StatusApi.md#status_status_get) | **GET** /status | Status


## Documentation For Models

 - [Application](docs/Application.md)
 - [HTTPValidationError](docs/HTTPValidationError.md)
 - [Node](docs/Node.md)
 - [Status](docs/Status.md)
 - [ValidationError](docs/ValidationError.md)


## Documentation For Authorization

 All endpoints do not require authorization.

## Author




