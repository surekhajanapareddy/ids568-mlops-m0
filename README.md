\# Milestone 0 - Environment \& CI Setup

[![CI](https://github.com/surekhajanapareddy/ids568-mlops-m0/actions/workflows/ci.yml/badge.svg)](https://github.com/surekhajanapareddy/ids568-mlops-m0/actions/workflows/ci.yml)


\[!\[CI](https://github.com/surekhajanapareddy/ids568-mlops-m0/actions/workflows/ci.yml/badge.svg)](https://github.com/surekhajanapareddy/ids568-mlops-m0/actions/workflows/ci.yml)



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



In addition to dependency pinning, this project includes a continuous integration (CI) workflow implemented with GitHub Actions. The CI pipeline automatically installs dependencies in a clean environment and runs a smoke test using pytest on every push or pull request. This validates that the environment setup works correctly outside the local system. Together, exact dependency pinning and automated testing improve reliability across the machine learning lifecycle by enabling repeatable experiments, early detection of issues, and smoother transitions from development to deployment.

