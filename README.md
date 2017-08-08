# isatools-notebooks

This repository contains notebooks to demonstrate the `isatools` software package.

Run locally:

Install Python requirements with `pip install -r requirements.txt`.

If your using `qgrid` in your notebook or in iPython, ensure the following lines are run:
```
import qgrid
qgrid.nbinstall(overwrite=True)
```
This copies some JavaScript that `qgrid` needs to render tables in Jupyter.

Ensure notebook extensions are enabled with `jupyter nbextension enable --py widgetsnbextension`

Start Jupyter Notebook with `jupyter notebook`

Or run using the dockerfile: `docker build -t isatools .` then `docker run -it -im -p 8888:888 isatools`

If you can't find your local Jupyter running, try `docker-machine ls` to get the IP instead of using `localhost:8888`.
