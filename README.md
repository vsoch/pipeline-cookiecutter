{{cookiecutter.project_name}} Encode Pipeline
=============================================

This is a work in progress, a template for an example repository. The documentation
will be found in this README until development is more finalized, and then move 
into a proper format.

# Usage

## Step 1. Generate Codebase

You can generate your starter ENCODE repository by doing the following:

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

At this point, you should customize the *.wdl file to coincide with your workflow. 
There are a set of nice examples provided [here](https://github.com/dnanexus/dxWDL/tree/master/test/basic).


## Step 2. Documentation

The template also includes documentation, which will render to Github pages based on being in the "docs"
folder. This means that once you push to Github, you should go to settings --> Github pages and
select the option to have the docs for the repository to render from the docs folder.


# Directories

* `backends/` : Backend configuration files (`.conf`)
* `workflow_opts/` : Workflow option files (`.json`)
* `examples/` : input JSON examples (SE and PE)
* `data/` : data TSV files for each platform
* `src/` : scripts for each task in WDL
* `docker/` : Dockerfile and MySQL DB initialization script
* `test/` : test scripts for developers
