{{cookiecutter.project_name}} Encode Pipeline
=============================================

This is a work in progress, a template for an example repository. You can
generate your starter ENCODE repository by doing the following:


## Usage

1. Install cookiecutter

```bash
pip install cookiecutter
```

2. Clone this repository

```bash
git clone https://www.github.com/vsoch/pipeline-template
```

3. Edit the cookiecutter.json file with your parameters.

```json
cd pipeline-template
cat cookiecutter.json
{
    "project_lead": "Vanessa Sochat",
    "project_email": "encode-help@lists.stanford.edu",
    "project_name": "Hello Cookie Pipeline Template",
    "project_slug": "pipeline-template",
    "repo_user": "vsoch",
    "repo_name": "pipeline-template",
    "project_short_description": "An encode pipeline cookie cutter template.",
    "year": "2018",
    "version": "0.0.1"
}
```

3. Create the repository from this one:

```bash
cookiecutter --no-input
```


# Directories

* `backends/` : Backend configuration files (`.conf`)
* `workflow_opts/` : Workflow option files (`.json`)
* `examples/` : input JSON examples (SE and PE)
* `data/` : data TSV files for each platform
* `src/` : scripts for each task in WDL
* `docker/` : Dockerfile and MySQL DB initialization script
* `test/` : test scripts for developers
