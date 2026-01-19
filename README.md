\# Milestone 0 - Environment \& CI Setup

[![CI](https://github.com/surekhajanapareddy/ids568-mlops-m0/actions/workflows/ci.yml/badge.svg)](https://github.com/surekhajanapareddy/ids568-mlops-m0/actions/workflows/ci.yml)


\## Setup (Windows)

```powershell

py -m venv .venv

.\\.venv\\Scripts\\Activate.ps1

python -m pip install --upgrade pip

pip install -r requirements.txt

pytest -v



