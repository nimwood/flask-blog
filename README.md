# flask-blog

A webproject using Flask as a webserver and Bootstrap for layout and styling

## Requirements

Running:
1. Python version 3.7.3
2. Flask `pip install flask`

Editor:
1. Download VSCode by Microsoft

Extensions you probably want:
1. IntelliSense for CSS class names in HTML

## Serve locally

Try to keep python versions the same and use python 3.7.3
run `python3.7.3 flask run`

## Set environment variables

If you want to use `flask run` you have to set two environment variables

Set so flask knows which file to run
`export FLASK_APP=flaskblog.py` in the project directory

Set so you don't have to re-run flask run after every change
`export FLASK_DEBUG=1` 

Windows use `set` instead of `export`

## Deployment instructions