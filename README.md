\# Milestone 0 - Environment \& CI Setup

[![CI](https://github.com/surekhajanapareddy/ids568-mlops-m0/actions/workflows/ci.yml/badge.svg)](https://github.com/surekhajanapareddy/ids568-mlops-m0/actions/workflows/ci.yml)


\[!\[CI](https://github.com/surekhajanapareddy/ids568-mlops-m0/actions/workflows/ci.yml/badge.svg)](https://github.com/surekhajanapareddy/ids568-mlops-m0/actions/workflows/ci.yml)

**Python version:** 3.11


\## Setup (Windows)

\## 1. Create virtual environment

```powershell

py -m venv .venv

```
\## 2. Activate virtual environment

```powershell

.\\.venv\\Scripts\\Activate.ps1

```
\## 3. Upgrade pip within the virtual environment

```powershell

python -m pip install --upgrade pip

```
\## 4. Install all project dependencies 

```powershell

pip install -r requirements.txt

```
\## 5. Smoke test to verify the environment setup 

```powershell

pytest -v

```


\## Reproducibility and Environment Setup

In this project, we emphasize reproducibility by ensuring that anyone can recreate the same software environment and verify results consistently. All Python dependencies are pinned to exact versions in requirements.txt using pip freeze, which prevents unexpected changes when installing packages on different machines. This approach avoids the common “it works on my machine” problem and ensures consistent behavior across development, testing, and deployment environments.

This project uses GitHub Actions to build a continuous integration (CI) process in addition to dependency pinning. Every time a push or pull request is made, the CI pipeline automatically installs dependencies in a clean environment and uses pytest to perform a smoke test. This confirms that the environment configuration functions properly outside of the local system. By facilitating repeatable experiments, early problem discovery, and more seamless transitions from development to deployment, accurate dependency pinning and automated testing work together to increase reliability throughout the machine learning lifecycle.
