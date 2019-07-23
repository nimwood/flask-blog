# flask-blog

A webproject using [Flask](https://palletsprojects.com/p/flask/) as a webserver and [Bootstrap](https://getbootstrap.com/docs/4.3/getting-started/introduction/) for layout and styling

## Requirements

Prefereably use Docker (see run using docker instructions)

OR

1. Python version 3.7.2
2. Flask `pip install flask`

Some other things you might want to use

Editor:
1. Download the best IDE which is [VSCode](https://code.visualstudio.com/) by Microsoft

Extensions you probably want:
1. IntelliSense for CSS class names in HTML

## Serve locally

Why is using docker more preferable? Basically you don't have to worry about dependencies, enviroment, versions or any of that crap. You just have a single image that runs anywhere.

### Run using Docker

If you can, run using Docker. This will make it so that our project works from all our different laptops and doesn't change functionality due to differences in environment

1. Download [Docker for Desktop](https://www.docker.com/products/docker-desktop)

2. Build the image

```docker build -t flask-app .```

3. Run a container

```docker run --rm -it -v ${PWD}:/app -p 5000:5000 flask-app```

Now you can go to ```localhost:5000``` in your browser to see the app

### Run on your machine

If you don't want to use Docker you can still run the Flask app using the normal methods

#### Easy method
Try to keep python versions the same and use python 3.7.2
run `python3 app.py`

#### Harder method
If you want to use `flask run` you have to set two environment variables

Set so flask knows which file to run
`export FLASK_APP=app.py` in the project directory

Set so you don't have to re-run flask run after every change
`export FLASK_DEBUG=1` 

Windows use `set` instead of `export`

## Deployment instructions