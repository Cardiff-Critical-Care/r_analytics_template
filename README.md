# Template for analytical projects using Python

## Pre-requisite

You must have git installed on your machine.

## Usage

All analytical projects must use a standard template. This one is for use when R is the chosen language. To get started, clone this repository to your local machine:

```bash
git clone https://github.com/Cardiff-Critical-Care/r_analytics_template.git
```

Rename the project folder with your project title e.g. 'TestProject'. Then associate your project with a GitHub repository on the teams GitHub account:

```bash
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/Cardiff-Critical-Care/TestProject.git
git push -u origin main
```

Now the project can be tracked for version control. 

For analytical projects we use Anaconda. Install the default conda environment using the YAML file:

```bash
conda env create -f conda_env.yml
```

Data must not be stored on GitHub! Keep project data in the 'data' folder. There are precautions in place using the gitignore config file and pre-commit to prevent data uploads, but it is the analysts reponsibility to make sure no unauthorised data is stored in GitHub repositories.
