---
title: "Lecture2 # Installing Docker: A Step-by-Step Guide for Linux Operating Systems"
datePublished: Fri Dec 08 2023 17:00:22 GMT+0000 (Coordinated Universal Time)
cuid: clpwvhu6u000008l5c8e56oi6
slug: lecture2-installing-docker-a-step-by-step-guide-for-linux-operating-systems
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1701887393662/a46e14aa-8961-47e5-95ff-ba88efd50004.png
tags: docker, devops, docker-images, devops-articles, masterwithhamza

---

Docker has become an integral part of modern software development, providing a platform for efficient containerization. This article offers detailed instructions, ensuring a smooth setup for Docker.

## **Installing Docker on Linux:**

### **Requirements:**

* Docker requires a 64-bit installation and a compatible Linux kernel.
    

### **Steps (Generic for Ubuntu-based systems):**

1. **Update Package Lists:** Open a terminal and update the package lists:
    

```bash
sudo apt-get update
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1702054353570/0d7e1b14-ffea-4342-b3c6-91d734aa0593.png align="center")

1. **Install Docker:** install the Docker.
    

```bash
sudo apt-get install docker.io
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1702054645397/f76dbeb4-6f2d-40fe-89fb-a7d085c04ab0.png align="center")

1. **Verify Installation:** Confirm that Docker is installed correctly by running the following command.
    

```bash
docker --version
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1702054728351/672e6ab8-de95-40f8-ab95-2558bfa39b74.png align="center")