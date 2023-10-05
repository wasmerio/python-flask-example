# Sample Python Flask Server with Wasmer

This is a sample repo for running a Python's Flask server on Wasmer Edge.

## Running it locally

### Clone the repo

```shell
git clone https://github.com/wasmerio/python-flask-example.git
```

### Setup the Virtual Environment

```shell
python3 -m venv .env
source .env/bin/activate
pip3 install Flask
```

### Run it locally using the command below

```shell
$ wasmer run . --net
 * Serving Flask app '/src/main'
 * Debug mode: on
WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
 * Running on http://127.0.0.1:5000
Press CTRL+C to quit
```

## Running it using wasmer registry

This package is published to wasmer registry as [`wasmer/python-flask-server`](https://wasmer.io/wasmer/python-flask-server)

You can try this locally.

```shell
$ wasmer run . --net
 * Serving Flask app '/src/main'
 * Debug mode: on
WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
 * Running on http://127.0.0.1:8080
Press CTRL+C to quit
```

This would start an http server on `http://127.0.0.1:8080`

![Python Flask Server](python-flask-server.png)

## Live on Wasmer Edge

You can check the app in: 
https://wasmer-python-flask-server-worker.wasmer.app