<!-- .slide: data-background-image="images/paul-teysen-bukjsECgmeU-unsplash.jpg" -->
# Introduction to Linux Containers

---

## Objectives

- This slide deck is an introduction to Linux Containers for non technical people.

- We won't run any container nor explore deep technical details on how containers are implemented here.

---

## The hype about Linux containers


- The way we develop software is evolving.

- Before (can still be current for some of us ...)
  - Monolithic application
  - Long development cycle (waterfall methodology)
  - Vertical scaling focused (add CPU, memory and disks aka run on a beefier hardware)

- Now:
  - loosely coupled services
  - _Agile_ development
  - Horizontal scaling (running multiple replicas)

---

## Deployment becomes more complex

- Many different stacks used

  - Languages
  - Frameworks (think .Net or Java version dependency)

- Many different targets:

  - individual development environments
  - test, QA, preproduction, ...
  - on-premises and/or cloud service provider

---

## The deployment problem

<img class="r-stretch" src="images/deployment_problem.png" />

---

## The deployment matrix from hell

![the deployment matrix from hell](images/deployment_matrix_hell.png)

---

## Parallel with the shipping industry

<img src="images/shipping_problem.png" width="650" height="560" />

---

## intermodal shipping containers

<img src="images/shipping_solution.png" width="650" height="560" />

---

## A new shipping ecosystem

<img class="r-stretch" src="images/new_shipping_ecosystem.png">

- 90% of all cargo is now shipped in standard containers
- faster load / unload of ships
- drastic reduction of losses due to theft and/or damages

---

## Containers for applications

<img class="r-stretch" src="images/deployment_solution.png" />

<div style="font-size: 16px; text-align: left;">

Warning: it is possible to package stateful applications like databases or message brokers in containers but it requires more expertise because data persistence in containers is tricky.

</div>

---

# Technical advantages

---

## No more dependency hell

<div style="text-align: left;">

Application packaging can be resumed to the following steps :


1. Define, test and document (example in `INSTALL.txt` file) installation instructions.

2. Create some installation script that works for you as developer.

3. Turn this into a `Dockerfile` (or a container build file).

4. Build the container image and test it.

5. If the container works on your machine, it will work on every other machines that can run containers.

</div>

---

## Other use cases for Linux containers

- Faster onboarding of new developers (package environments as containers).

- Implement better _Continuous Integration_ (containers are faster to create than VMs and leave your CI environment clean).

- Use container images as build artefacts, store them in registry with multiple versions (enables easy rollback in case of issue), deploy the same image in all environments.

---

# Last info

---

## Container engines

- Container engines provide 3 important things to ease the use of containers
  
  1. User interface / API.

  1. Capability to push / pull container images.

  1. Create JSON configuration file for container runtimes (the tool that effectively runs the container).

- Most known container engine is [Docker](https://www.docker.com/), but other alternatives like [podman](https://podman.io/) or [LXD](https://linuxcontainers.org/lxd/introduction/) are growing fast due to some issues with the Docker implementation.

---

<!-- .slide: data-background-image="images/paul-teysen-bukjsECgmeU-unsplash.jpg" -->
# That's all folks




