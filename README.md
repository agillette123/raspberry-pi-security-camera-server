# Web Server to preserve camera images on Render.com

## Setup of local environment on your machine (not a raspberry pi)

### Clone this repo

    git clone 

### Create a virtual environment

```bash
python3 -m venv ./venv-server
source venv-server/bin/activate
```

### Install the dependencies

    pip install -r requirements.txt


### Development mode run server

    gunicorn main:app -b 127.0.0.1:5000 --reload


### Production mode run server

    gunicorn main:app -b 0.0.0.0:8080

### Flask and flask example license https://flask.palletsprojects.com/en/2.1.x/license/#bsd-3-clause-source-license