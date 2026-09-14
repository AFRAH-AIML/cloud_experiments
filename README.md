# Cloud Computing Lab — Experiments 1–7

This repository contains the implementation, configurations, and documentation for a **Cloud Computing Laboratory** covering virtualization, cloud application development, object storage, cloud simulation, and virtual machine networking.

The experiments are designed to demonstrate fundamental cloud concepts using practical, hands-on tools such as **VirtualBox, Ubuntu, Google Cloud CLI, Flask, MinIO, CloudSim, Maven, IntelliJ IDEA, and Vagrant**.

---

## 📚 Experiments

### Experiment 1 — Virtual Machine Creation with VirtualBox

**Objective:**
Set up a virtualized Linux environment using Oracle VirtualBox.

The experiment covers:

* Installing Oracle VM VirtualBox
* Downloading an Ubuntu Desktop ISO
* Creating and configuring an Ubuntu virtual machine
* Allocating RAM and virtual disk space
* Installing and booting Ubuntu

**Concepts:** Virtualization, Virtual Machines, Hypervisors, Resource Allocation

---

### Experiment 2 — C Compiler in a Virtual Machine

**Objective:**
Install and use the GCC compiler inside the Ubuntu virtual machine.

The experiment demonstrates:

* Updating Ubuntu packages
* Installing `build-essential`
* Verifying GCC
* Creating a simple C program
* Compiling and executing the program

Example output:

```text
Hello, Virtual Cloud World!
```

**Concepts:** Virtualized development environments, compilers, Linux development tools

---

### Experiment 3 — Google Cloud CLI & App Engine Setup

**Objective:**
Set up the Google Cloud CLI and prepare a simple Python application for Google App Engine.

The experiment covers:

* Installing Google Cloud CLI
* Initializing and authenticating `gcloud`
* Selecting a Google Cloud project
* Installing the App Engine Python component
* Creating a Python application
* Configuring `app.yaml`
* Defining application dependencies

The implementation uses a currently compatible Python runtime instead of the outdated runtime specified in the original lab material.

**Concepts:** Cloud platforms, PaaS, Google App Engine, cloud application configuration

---

### Experiment 4 — Launching a Flask Web Application

**Objective:**
Run the Python web application locally using Flask.

The experiment demonstrates:

* Creating a Python virtual environment
* Installing project dependencies
* Managing Flask and Werkzeug versions
* Running the application
* Accessing the web application through a browser

Expected output:

```text
Hello world from Google App Engine!
```

**Concepts:** PaaS application development, Python environments, Flask, web services

---

### Experiment 5 — Cloud Object Storage with MinIO

**Objective:**
Build a local S3-compatible object storage environment using MinIO and Python.

The application implements:

* Bucket creation
* Object upload
* Object download
* Object listing
* Metadata display
* Object deletion

A Python-based interactive **Object Storage Manager** communicates with the local MinIO server using the official MinIO Python SDK.

**Concepts:** Object storage, buckets, object keys, metadata, S3-compatible APIs

---

### Experiment 6 — CloudSim with SJF Scheduling

**Objective:**
Simulate a cloud computing environment using CloudSim and implement **Shortest Job First (SJF)** scheduling.

The experiment covers:

* Installing Java, Git, Maven, and IntelliJ IDEA
* Setting up CloudSim
* Creating a simulated datacenter
* Creating VMs and Cloudlets
* Implementing a custom `SJFDatacenterBroker`
* Sorting Cloudlets according to their execution length
* Running and verifying the simulation

The demonstrated execution order is:

```text
10000 MI → 20000 MI → 40000 MI
```

**Concepts:** Cloud simulation, Cloudlets, VMs, brokers, scheduling algorithms, SJF

---

### Experiment 7 — File Transfer Between Virtual Machines

**Objective:**
Create two lightweight virtual machines and transfer a file between them over a virtual network.

The experiment uses **Vagrant + VirtualBox** to create:

```text
VM1 → 192.168.56.10
VM2 → 192.168.56.11
```

The workflow includes:

* Creating a VirtualBox network
* Configuring a Vagrant environment
* Creating two Ubuntu VMs
* Assigning network addresses
* Testing connectivity using `ping`
* Creating a file on VM1
* Transferring the file to VM2
* Verifying the transferred file

**Concepts:** IaaS, virtual networking, VM-to-VM communication, file transfer

---

## 🛠️ Technologies Used

| Technology        | Purpose                    |
| ----------------- | -------------------------- |
| Oracle VirtualBox | Virtualization             |
| Ubuntu            | Guest operating system     |
| GCC               | C compilation              |
| Google Cloud CLI  | Cloud platform interaction |
| Google App Engine | Application platform       |
| Python / Flask    | Web application            |
| MinIO             | Object storage             |
| MinIO Python SDK  | Storage API                |
| CloudSim          | Cloud simulation           |
| Java / Maven      | CloudSim development       |
| IntelliJ IDEA     | Java development           |
| Vagrant           | Automated VM management    |

---

## 🧩 Overall Learning Path

```text
Virtualization
      ↓
Linux Development Environment
      ↓
Cloud Platform & Web Application
      ↓
Cloud Object Storage
      ↓
Cloud Simulation & Scheduling
      ↓
Virtual Networking & VM Communication
```

Together, the seven experiments provide a practical introduction to the major building blocks of cloud computing — from **virtual machines and cloud applications to storage, simulation, networking, and resource scheduling**.

---

## 📁 Suggested Repository Structure

```text
cloud-computing-lab/
│
├── Experiment-1-VirtualBox/
├── Experiment-2-GCC/
├── Experiment-3-Google-App-Engine/
├── Experiment-4-Flask-App/
├── Experiment-5-MinIO-Object-Storage/
├── Experiment-6-CloudSim-SJF/
├── Experiment-7-Vagrant-File-Transfer/
│
├── screenshots/
│
├── Lab-Manual/
│   └── Consolidated-Lab-Manual.pdf
│
└── README.md
```

## 🎯 Result

All **seven cloud computing experiments** were successfully implemented and verified, covering virtualization, cloud application development, object storage, cloud simulation, scheduling, virtual networking, and VM-to-VM file transfer.
