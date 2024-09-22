# Machine Learning Demo Project

A sample end-to-end machine learning project, based on a [Feature Store Liveproject](https://www.manning.com/liveproject/creating-features) on manning.com.

### Prerequisites

- [Py Launcher](https://python-launcher.app/install/)
- [Pip Compile](https://pip-tools.readthedocs.io/en/stable/)

### Project Setup

1. Create a virtual env with desired version of Python
   1. Example, with `py-launcher`
   2. `py -3.11 -m venv .venv`
2. Install dependencies
   1. `py -m pip install -r requirements.txt`

### Adding Dependencies

1. Use `pip-compile` to generate a new `requirements.txt`
   1. `py -m pip install pip-tools`
   2. Add dependency to `requirements.in`
   3. Run `pip-compile requirements.in`

### Project Structure

This is intended as a learning project.  Several different machine learning models are used and trained on the diabetes dataset.  

The `/caches` folder has cached versions of machine learning models used in the project.

The `/feature_store` folder has a demo implementation of the feature store pattern.  The feature engineering output is stored in CSV files instead of in a database.