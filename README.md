# CI/CD with Tekton and OpenShift

This repository contains the implementation of a CI/CD pipeline project that integrates **GitHub Actions**, **Tekton**, and **OpenShift** to demonstrate modern DevOps practices.

---

## Objectives

* **GitHub Actions CI Pipeline**

  * Create a workflow with steps for linting and unit testing.

* **Tekton Tasks**

  * Define tasks for linting, unit testing, and building a container image.

* **OpenShift CI Pipeline**

  * Create an OpenShift pipeline that reuses the Tekton tasks.

* **Deployment Step**

  * Extend the OpenShift pipeline to deploy the application to an OpenShift cluster.

---

## Usage

This repository is designed as a standalone project.
To get started, clone the repo into your own GitHub account:

```bash
git clone https://github.com/<your-username>/CI-CD_with_Tekton.git
```

---

## Setup

Inside your lab or local environment, install prerequisites by running:

```bash
bash bin/setup.sh
```

After installation, restart the shell to activate the Python virtual environment:

```bash
exit
```

---

## Tasks

### 1. GitHub Actions Pipeline

* Configure a workflow under `.github/workflows/`
* Jobs include:

  * **Linting** (code quality checks)
  * **Unit Testing** (validating application logic)

### 2. Tekton Tasks

* Create Tekton `Task` definitions for:

  * Linting
  * Unit Testing
  * Image Build

### 3. OpenShift Pipeline

* Define an OpenShift pipeline that **reuses Tekton tasks**.

### 4. Deployment

* Add a deployment step to the OpenShift pipeline to roll out the application to the lab OpenShift cluster.

---

## License

This project is licensed under the [Apache License](LICENSE).

---

## Author

Created and maintained by **Abdullah Siraj**
