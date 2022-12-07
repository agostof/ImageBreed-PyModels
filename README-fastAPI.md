## Overview

## ImageBreed-BrAPI-FastAPI: Python-based ImageBreed with Breeder's API-Like (BrAPI) server stubs and data models

* Includes models and server stubs (views.py) 
* Use as a template to create your Python-based [ImageBreed-BrAPI server]
* Use models to create a [ImageBreed-BrAPI client](client/barebones_brapi_client.py) (a.k.a *BrAPP*) or to create a client library.
* Integrate models with other Python frameworks.


## Quick start
1. Installation using pyenv, skip this step if you don't want to use pyenv.
``` sh
pyenv virtualenv 3.9.1 WebAPI
pyenv activate WebAPI
```
2. Install module dependencies
``` sh
python -m pip install -r requirements.txt
```
3. Then start server
``` sh
cd server
./start_dev_server.sh
```
The local server should be running at `port 9000`, to see available endpoints visit your serverinfo endpoint: http://127.0.0.1:9000/brapi/v2/serverinfo.

Details for how to [implement an endpoint](server/README.md#implementing-brapi-endpoints), and a list of the implemented example endpoints are available in the [server's README](server/README.md).

### Auto-generated documentation
The default **FastAPI** server will generate and display documentation for your running instance using **Swagger UI** and **ReDoc**. This documentation will be available at `{server_url}/docs` or `{server_url}/redocs`. Check the [server's README](server/README.md) for details.


