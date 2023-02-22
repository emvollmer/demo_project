# demo_project
[![Build Status](https://jenkins.indigo-datacloud.eu/buildStatus/icon?job=Pipeline-as-code/DEEP-OC-org/UC-emvollmer-demo_project/master)](https://jenkins.indigo-datacloud.eu/job/Pipeline-as-code/job/DEEP-OC-org/job/UC-emvollmer-demo_project/job/master)

Testing cookiecutter tool following video "Tutorial - Module development"

To launch it, first install the package then run [deepaas](https://github.com/indigo-dc/DEEPaaS):
```bash
git clone https://github.com/emvollmer/demo_project
cd demo_project
pip install -e .
deepaas-run --listen-ip 0.0.0.0
```
The associated Docker container for this module can be found in https://github.com/emvollmer/DEEP-OC-demo_project.

## Project structure
```
├── LICENSE                <- License file
│
├── README.md              <- The top-level README for developers using this project.
│
├── requirements.txt       <- The requirements file for reproducing the analysis environment, e.g.
│                             generated with `pip freeze > requirements.txt`
│
├── setup.py, setup.cfg    <- makes project pip installable (pip install -e .) so
│                             demo_project can be imported
│
├── demo_project    <- Source code for use in this project.
│   │
│   ├── __init__.py        <- Makes demo_project a Python module
│   │
│   └── api.py             <- Main script for the integration with DEEP API
│
└── Jenkinsfile            <- Describes basic Jenkins CI/CD pipeline
```
