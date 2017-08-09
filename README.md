# isatools-notebooks

This repository contains notebooks to demonstrate the `isatools` software package.

## To run locally:

#### In the terminal window

Install Python requirements with `pip install -r requirements.txt`.

#### In Python

If your using `qgrid`, either in your Jupyter Notebook or in a Python or iPython console, ensure the following lines are run once to make sure `qgrid` is fully installed into your Jupyter instance:
```
import qgrid
qgrid.nbinstall(overwrite=True)
```
This copies some JavaScript that `qgrid` needs to render tables in Jupyter. [See here](http://nbviewer.jupyter.org/gist/TimShawver/8fcef51dd3c222ed25306c002ab89b60#Notebook-installation) for further clarification.

#### In the terminal window again

Before starting Jupyter (or if you did the previous step inside Jupyter, exit Jupyter first and return to the terminal prompt), please ensure notebook extensions are enabled with `jupyter nbextension enable --py widgetsnbextension`.

Start Jupyter Notebook with `jupyter notebook`. This should automatically spawn a browser Window running Jupyter. If it does not, in the terminal window it will give you a link in some text like:

```
    Copy/paste this URL into your browser when you connect for the first time,
    to login with a token:
        http://localhost:8888/?token=cf7362977cda558549f13d5a8d40b6929a6c49700a36d56b
```

*Hint: On MacOS if `jupyter notebook` does not automatically open the browser for you, try run `export BROWSER=open` first. You can add this `EXPORT` line to your `~/.bash_profile`.

## Alternatively

Or run using the dockerfile: `docker build -t isatools .` then `docker run -it -im -p 8888:888 isatools`

If you can't find your local Jupyter running, try `docker-machine ls` to get the IP instead of using `localhost:8888`.
