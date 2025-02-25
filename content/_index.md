+++
title = "Reproducible Research Experiments"
outputs = ["Reveal"]
+++

# Reproducible Experiments 
# in Computer Science Research
## Martina Baiardi and Raphael Schwinger

---

# Table of Contents
## **Slide to be removed**

1. Introduction to reproducible research meaning (**Martina**)
2. Reproducibility starts from development: build tools (gradle x JVM, Poetry x Python) and frameworks (hydra) (**Raphael**)
3. Basics of Containerization: Dockerfile and docker-compose (**Martina**)
4. Hands on a project: RL reproducible experiment setup using Poetry and Hydra (**Raphael**)
5. Cherry on the top: automation. GitHub, OSS proj, CI/CD pipelines, Github Actions, ... (**Martina**)

---

# What is reproducibility?

{{% multicol %}}{{% col %}}

Reproducibility of experiments is the key to validating scientific claims.

1. **Validation of Results** that were claimed in the scientific publication
2. **Advancing Knowledge** without re-building everything from scratch

{{% /col %}}{{% col class="text-center" %}}

<img src="images/building-blocks.svg" width=60%/>

{{% /col %}}{{% /multicol %}}

---

# How does this affect us as computer scientist?
## Let's make an example

* I find an interesting paper that fits my research needs.

* The authors' methods seem perfect for my work, so I want to dive deeper into their experiment.

* I look for the companion artifact... <b> What can go wrong? </b>

---

# 1) Artifacts not available


The link to the research artifacts (code, data, etc.) is broken.


<img class="inline-block" src="images/github.png" width=40%/>
<img class="inline-block" src="images/zenodo.png" width=25%/>

---

# 2) Missing an explanation on how to execute it

* The artifacts are available but in non-standard formats that researchers can be unfamiliar with.
* The file sizes are unexpectedly large.
* No clear instructions on how to use them.

<br/>
<br/>

> Example: How would you open and execute a `duffy-duck.qcow2` file that weights 20GB? Yes, it can be a valid artifact.

---

# 3) The artifact is not running 

* Strange errors prevent the artifact to execute on my pc
* Runtime dependencies may be missing, but `which` ones?

--- 

## Moreover, let's don't forget about
## the elephant in the room

<img class="inline-block" src="images/gpt-papers.png" width=80%/>

--- 

# As computer scientists we can do better

{{% fragment %}}

Reproducibility starts from development:
1. **Reproducible builds**: Adoption of build automation <br/> tools to manage experiment dependencies.
2. **Isolation**: Prepare a lightweight containerized environment <br/> for the distribution of the experiment.
3. **Automation**: Create an automatic pipeline that tests <br/> the source-code and generates the artifacts, <br/>so you don't have to do it by hand.
4. **Open-Source Research**: protect your ownership <br /> by picking correct license.    

{{% /fragment %}}

---

# Build automation tools

Raphael you can continue here

---

# Containerization

---


--- 

# Hands on a real example! 

Raphael you can continue here

---

# Cherry on the top

---


