---
title: JupyterHealth
site:
  hide_outline: true
---

**Open infrastructure for health care.**
JupyterHealth is a secure, connective layer for bringing wearable, clinical, and {term}`patient-generated data` into modern computational and AI-enabled health care workflows.
It is open source, built on open standards like {term}`FHIR` and {term}`Open mHealth`, and made for researchers, clinicians, and patients.
It has three main pieces:

- The {term}`Exchange` stores {term}`patient-consented data` and serves it through REST, FHIR, and {term}`MCP` APIs.
- The {term}`Hub` is where researchers and data scientists analyze that data, and the platform for building and deploying dashboards and apps for clinicians and other downstream users.
- The {term}`client library` reads Exchange data from Python for analysis and re-use.

This site describes the project at a high level and points to each component's documentation.
Read [About the project](about.md) for its origins and primary materials.

:::{note} JupyterHealth is under active development
These pages describe what the project is building toward. Some pieces are further along than others.
:::

## What do you want to do?

::::{grid} 1 1 2 2

:::{card} Analyze data and build dashboards on the Hub
:link: https://jupyterhealth-hub.readthedocs.io/en/latest/
Log in to the {term}`Hub` with your {term}`Exchange` account, pull data into a notebook with the client library, and run your own analyses.
:::

:::{card} Write Python that uses data from the Exchange
:link: https://jupyterhealth-client.readthedocs.io
The {term}`client library` returns observations as pandas DataFrames.
The [{term}`CGM` tutorial](https://jupyterhealth.github.io/software-documentation/tutorial/tutorial-cgm) is an end-to-end example.
:::

:::{card} Run the Exchange for your organization
:link: https://jupyterhealth.github.io/software-documentation/
Deploy your own {term}`Exchange`.
The docs cover setup, access control, the FHIR API, and the data model.
:::

:::{card} Deploy an app that uses the Exchange
:link: https://github.com/jupyterhealth/jupyterhealth-sof-provider-template
The linked repository lets you turn a notebook into a Voilà application. It can be served either on the {term}`Hub` or as a standalone app that an {term}`EHR` opens with {term}`SMART on FHIR`.
:::

::::
