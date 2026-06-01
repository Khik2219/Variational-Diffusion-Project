# Phase-3-Variational-Diffusion

Swat GPU Devices
or run nvidia-smi
https://status.cs.swarthmore.edu/grafana/d/cHtStXSVz/gpu-overview?orgId=2&refresh=5m

## Environment setup

From the repo root, create and activate the Python environment:

```bash
python -m venv /scratch/$USER/VDMkernel-env
source /scratch/$USER/VDMkernel-env/bin/activate
```

Install the required packages:

```bash
python -m pip install --upgrade pip setuptools wheel
python -m pip install -r requirements.txt
```

Register the environment as a Jupyter kernel:

```bash
python -m pip install ipykernel
python -m ipykernel install --user --name VDMkernel --display-name "VDMkernel"
```

In Jupyter, select the kernel named:

```text
VDMkernel
```

## Checking the active environment

Inside a notebook, run:

```python
import sys
print(sys.executable)
```

It should point to:

```text
/scratch/your_username/VDMkernel-env/bin/python
```

## GPU notes

To check GPU usage on the machine:

```bash
nvidia-smi
```

The Swarthmore GPU dashboard is listed above.
