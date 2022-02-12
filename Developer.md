# Development notes

Following are the notes for working on the development of the component.

## Quickstart for development

- In terminal 1
```shell
$ cd st_barfi/frontend
$ npm run serve
```

- In terminal 2
```shell
$ streamlit run st_barfi/__init__.py 
```

## Requirements

- Ensure you have [Python 3.6+](https://www.python.org/downloads/), [Node.js](https://nodejs.org), and [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) installed.
- Clone this repo to a local folder.

## Python virtual environment

Create a new Python virtual environment:

```shell
$ python3 -m venv venv  # create venv
$ . venv/bin/activate   # activate venv
$ pip install streamlit # install streamlit
```

Run the components's Streamlit app:

```shell
$ . venv/bin/activate  # activate the venv you created earlier
$ streamlit run st_barfi/__init__.py  # run the root test
```

## Node environment

Install and initialize the component's frontend:

```shell
$ cd st_barfi/frontend
$ npm install    # Install npm dependencies
$ npm run serve  # Start the dev server
```

# Build and Deploy

```shell
pip isntall build twine
python -m build 
twine upload --verbose --skip-existing dist/*
```

## Resources

- https://stackoverflow.com/questions/1301346/what-is-the-meaning-of-single-and-double-underscore-before-an-object-name
- https://stackoverflow.com/questions/972/adding-a-method-to-an-existing-object-instance
- https://stackoverflow.com/questions/52799985/python-change-bound-method-to-another-method
- https://docs.python.org/3/tutorial/classes.html