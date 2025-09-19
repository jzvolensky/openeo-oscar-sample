# openEO run_oscar process sample

This repository contains a sample tutorial on how to use the new run_oscar process in openEO.

## Prerequisites

This is still in development so you need to install the proper branch of `openeo-processes-dask` and `openeo local processing`

Clone the correct branch of `openeo-processes-dask`:

```bash
git clone --recurse-submodules -b run_oscar git@github.com:jzvolensky/openeo-processes-dask.git
```

```bash
cd openeo-processes-dask

poetry install --all-extras
```

Activate the virtual environment for processes-dask and install the local processing package:

```bash
pip install "openeo[localprocessing]"
```

Copy the the latest `run_oscar` process spec into the specs

```bash
curl -L -o openeo-processes-dask/openeo_processes_dask/specs/openeo-processes/run_oscar.json https://raw.githubusercontent.com/jzvolensky/openeo-processes/run_oscar/run_oscar.json

Then navigate to `OSCAR/openeo_oscar_dummy.ipynb` and enjoy. You may need to tweak your text editor settings to find the virtual environment as its not in the default location this way.


