# Docker Lab: Containerizing a Three-Tier Application
**INET 4031 - Introductions to Systems**

This lab introduces Docker and Docker Compose by having you containerize a
real, multi-service application. You will package three components: Apache,
Flask, and MariaDB. These will be packaged into separate containers and wired together so they function as a complete application.

The application code and scaffolding are provided. Your job is to complete the Dockerfiles, verify the stack runs correctly, and document your work below.

> **Directions and explanations for this lab are on the repository Wiki.**
> Refer to the Wiki pages for step-by-step instructions.

---

*The sections below are for you to fill out. Replace each placeholder with your own content before submitting. Having a detailed README is the best practice for showing your work in future GitHub repositories.*

---

# Project Overview

<!-- Briefly describe what this application does in your own words.
     What problem does it solve? What does a user interact with? -->
The project implements a simple ticket system, It allows user to view, create and manage tickets through a web or API.
the system solves organizing and tracking issues automatically.
# Prerequisites

<!-- List what needs to be installed or configured on the VM before this lab
     will work. Include Docker, Docker Compose, and anything else required. -->

This project requires docker, docker compose, git, and a Ubuntu enviroment to build an app supported by containters.

# Getting Started

<!-- Explain how a new teammate would bring this stack up from a fresh clone.
     Walk through every command they need to run, in order. -->
```bash
git clone <this repo's URL>
```

```bash
cd inet 4031 testlab12
```
```bash
cp .env.example .env
```
```bash
docker-compose up --build
```
After all of that, go to localhost and verify.

# Configuration

<!-- Explain the .env file: what it is, what variables it contains,
     and what a teammate needs to provide that is not in this repository. -->
.env file will be your task to create.
It contains 4 parameters given by the provided .env.example
Putting credentials there with such guided format.
# Verification

<!-- Describe how to confirm the stack is running correctly.
     Reference the check script and what a passing run looks like. -->
check the status of the container
restart the database after shutting it down via docker compose down.
(docker compose up --build)git push -u origin main
ran ./check-lab.sh to see if it passes the case
# Feedback (Optional)

<!-- Do you have any feedback you would like to give us after completing this lab? What are some things you enjoyed? What about others that you felt was lackluster? Or maybe there was something that we missed that you'd love for us to touch on! This will help us improve the INET 4031 lab experience. We appreciate everything we can get!  -->
