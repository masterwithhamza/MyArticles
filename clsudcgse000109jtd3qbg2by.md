---
title: "Docker Commands: A Comprehensive Guide"
datePublished: Tue Feb 20 2024 12:55:53 GMT+0000 (Coordinated Universal Time)
cuid: clsudcgse000109jtd3qbg2by
slug: docker-commands-a-comprehensive-guide
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1708433720362/94c4c28e-8a72-4a40-af15-29cd15c9d7ee.png

---

Docker has revolutionized the way developers build, ship, and run applications by enabling containerization. Docker containers provide a lightweight, portable, and isolated environment for running applications consistently across different platforms.In this guide, we'll explore Docker commands.

### **Basic Docker Commands:**

1. **docker run**: The fundamental command to create and start a container based on an image.
    

```bash
docker run nginx
docker run --name my-nginx -d -p 8080:80 nginx
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1708430734701/64af844c-711e-4e8e-8ba0-9e387668408d.png align="center")

**docker ps**: Lists all running containers.

```bash
docker ps
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1708430910785/5a187ccd-9868-4122-a20c-cb2faf24ff32.png align="center")

**docker images**: Lists all locally available Docker images.

```bash
docker images
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1708430976427/4fe6f5b0-3a13-41f9-a85e-413fa2273b63.png align="center")

**docker pull**: Fetches an image from a registry.

```bash
docker pull nginx
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1708432431260/2350c9f2-7013-4c17-8e27-e8f32e8c5f80.png align="center")

**docker build**: Builds an image from a Dockerfile.

```bash
docker build -t <image_name> <path_to_Dockerfile>
```

**docker stop**: Stops a running container.

```bash
docker stop <container_id>
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1708432648196/49294ce5-b5d4-4a9d-8cce-94b045f7ded3.png align="center")

**docker start**: Starts a stopped container.

```bash
docker start <container_id>
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1708432713211/cadd3e24-4005-462b-983c-db56a59df933.png align="center")

**docker restart**: Restarts a container.

```bash
docker restart <container_id>
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1708432778155/4c71dddf-10aa-4c8c-b0c4-265f7c52a677.png align="center")

**docker logs**: Retrieves the logs of a container.

```bash
docker logs <container_id>
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1708432912364/9c0d4cfe-3703-475c-9f1e-531e7e99488d.png align="center")

**docker inspect**: Provides detailed information about a container or image.

```bash
docker inspect <container_or_image_id>
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1708432997329/09afb5bd-d138-4042-9904-309eae4069d8.png align="center")

**docker rm**: Removes one or more stopped containers.

```bash
docker rm <container_id>
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1708433134447/f7e50fd8-0063-4e5d-895a-f0c18476573b.png align="center")

**docker rmi**: Removes one or more Docker images.

```bash
docker rmi <image_id>
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1708433270550/9553b4ca-0834-4a19-ac7f-ba60f01ca0da.png align="center")