---
layout: default
title: "The Scientific Filesystem"
pdf: true
permalink: /
---

<div style="float:right; margin-bottom:50px; color:#666">
Version: <a href="/spec-v1">{{ site.version }}</a><br>
Date: 2018-01-08
</div>

<div>
    <img src="img/logo/scif-slash-green.png" width="300px" style="float:left">
    <h1 style="margin-top:10px">Scientific Filesystem</h1>
</div><br><br>

Here we present the Scientific Filesystem (SCIF), an organizational format that supports exposure of executables and metadata for discoverability. The format includes a known *filesystem structure*, a definition for a set of *environment variables* describing it, and *functions* for generation of the variables and interaction with the libraries, metadata, and executables located within. Some quick resources:

 - [quick start](/tutorial-quick-start) or [really quick start](/tutorial-really-quick-start) tutorials to understand the format.
 - [Scientific Filesystem Container Builder](https://sci-f.github.io/builder) a `build` --> `test` --> `deploy` template to quickly turn your analysis scripts into a reproducible container.

## How does scif related to containers?
Although scif is not exclusively for containers, in that a container can provide an encapsulated, reproducible environment, the scientific filesystem works optimally when contained. Containers traditionally have one entrypoint, one environment context, and one set of labels to describe it. A container created with a Scientific Filesystem can expose *multiple* entry points, each that includes its own environment, metadata, installation steps, tests, files, and a primary executable script. SCIF thus brings internal modularity and programatic accessibility to encapsulated, reproducible environments.


## What will I learn reading this?
We will start by reviewing the background and rationale for a scientific organizational format, and how SCIF achieves the goals of **modularity**, **transparency**, and **consistency**. We then review the organizational structure of the standard, and the different levels of internal modules that it affords. For this work, we provide several tutorials to demonstrate using the scientific filesystem with Docker and Singularity, and additionally have implemented and released the organizational format as a native integration with the Singularity software. Finally, we discuss use cases for SCIF in context of containers, including how SCIF can be used to evaluate software, provide metrics, serve scientific workflows, and execute a primary function under different contexts. To encourage collaboration and sharing of apps, we have developed an open source, version controlled, tested, and programmatically accessible web infrastructure at <a href="https://sci-f.github.io/apps" target="_blank">https://sci-f.github.io/apps</a>. For developers, we provide a getting started guide for integration of SCIF into other container technologies or contexts. The ease of using SCIF to develop scientific containers offers promise for scientists to easily generate self-documenting containers that are programmatically parseable, exposing software and associated metadata, environments, and files to be quickly found and used. 


### Getting Started

 - [Tutorials](/tutorials): are a good place to start if you are a user or developer. These pages will show you how you generate and interact with a scientific filesystem. Or jump right in to a *[quick start](/tutorial-quick-start)* or *[really quick start](/tutorial-really-quick-start)*.
 - [Goals](/goals): here we review how SCIF allows for internal modularity and consistency, transparency, and reproducible practices.
 - [Examples](/examples): Whether you are a system admin, a developer, or a research scientist, why would you want to use SCIF anyway?
 - [Specification](/spec): reviews the current specification for SCIF.

### Resources

 - [Community](/community): community resources including APIs, version control and testing, and open source forums for tracking issues and discussion related to SCIF and scientific filesystem apps.
 - [Python Client](https://www.github.io/vsoch/scif): The SCIF client is the quickest start to creating and using scientific filesystems. Choose this client if you want interactivity, or are more comfortable with Python.
 - [GoLang Client](https://www.github.io/sci-f/scif-go): is the equivalent GoLang library, intended for integration with other GoLang libraries.
 - [Builder](https://sci-f.github.io/builder) the Scientific Filesystem Container Builder


We have provided several <a href="https://sci-f.github.io/apps/category/#Example" target="_blank">examples and tutorials</a> for getting started with SCIF. If you have a workflow or container that you'd like to see added, please <a href="https://www.github.com/sci-f/apps/issues" target="_blank">reach out</a>. If you would like to see other ways to contribute, <a href="/community.html#contribute-to-scif">here are some suggestions</a>. This work will remain open for contributions, and early contributions will be represented in an official submission.

### Citation
If SCIF has been useful to you, please cite our work on [GigaScience](https://academic.oup.com/gigascience/advance-article/doi/10.1093/gigascience/giy023/4931737)!

```
Vanessa Sochat; The Scientific Filesystem (SCIF), GigaScience, giy023,
https://doi.org/10.1093/gigascience/giy023
```

<div>
    <a href="/goals"><button class="next-button btn btn-primary"><i class="fa fa-chevron-right"></i> </button></a>
</div><br>
