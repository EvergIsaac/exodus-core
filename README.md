# εxodus core
[![Build Status](https://travis-ci.org/Exodus-Privacy/exodus-core.svg?branch=v1)](https://travis-ci.org/Exodus-Privacy/exodus-core) [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Exodus-Privacy/exodus-core.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Exodus-Privacy/exodus-core/context:python)

Contains:
* Static analysis
* Network analysis
* Connection helper

## Installation

exodus-core is available from [PyPI](https://pypi.org/project/exodus-core):
```
pip install exodus-core
```

## Include it to your project

Add the following line in your `requirements.txt` (replace 'XX' by the desired subversion):
```
exodus-core==XX
```

## Local usage

Clone this repository:
```
git clone https://github.com/Exodus-Privacy/exodus-core.git
cd exodus-core
```

### Using Docker

Build the Docker image:
```
docker build -t exodus-core .
```

Run tests:
```
docker run -it --rm exodus-core /bin/bash
python -m unittest discover -s exodus_core -p "test_*.py"
```

### Manual installation

Install `dexdump`:
```
sudo apt-get install dexdump
```

Create Python `virtualenv`:
```
virtualenv venv -p python3
source venv/bin/activate
```

Install dependencies:
```
pip install -r requirements.txt
```

Run tests:
```
python -m unittest discover -s exodus_core -p "test_*.py"
```
