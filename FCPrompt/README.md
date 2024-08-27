# How to Run

## How to Install
This code is built on top of the toolbox [Dassl-FCPrompt]. You can prepare the environment as follows:

```
cd Dassl-FCPrompt/

# Create a conda environment
conda create -n dassl python=3.7

# Activate the environment
conda activate dassl

# Install dependencies
pip install -r requirements.txt

# Install torch (version >= 1.7.1) and torchvision
# Please make sure you have installed the gpu version due to the speed.
# For example:
conda install pytorch torchvision cudatoolkit=10.1 -c pytorch

# Install this library (no need to re-build if the source code is modified)
python setup.py develop
```

After that, run `pip install -r requirements.txt` under `FCPrompt/` to install a few more packages required by [CLIP](https://github.com/openai/CLIP) (this should be done when `dassl` is activated). Then, you are ready to go.

Follow [DATASETS.md](DATASETS.md) to install the datasets.

# FCPrompt

```bash
cd FCPrompt/
```

Start to train FCPrompt:
```bash
bash scripts/run.sh
```

Get the evaluation results"
```bash
bash scripts/parse_run.sh
```
