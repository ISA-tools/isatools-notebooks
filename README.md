# isatools-notebooks

This repository contains notebooks to demonstrate the `isatools` software package.

Run locally: `pip install -r requirements.txt`, enable extensions `jupyter nbextension enable --py --sys-prefix widgetsnbextension` and then `jupyter notebook`

Or run using the dockerfile: `docker build -t isatools .` then `docker run -it -im -p 8888:888 isatools`

If you can't find your local Jupyter running, try `docker-machine ls` to get the IP instead of using `localhost:8888`.
