---
title: "Lecture7 # Efficient Disk Space Monitoring with a Shell Script"
datePublished: Fri Oct 20 2023 17:32:31 GMT+0000 (Coordinated Universal Time)
cuid: clnyw2g86000108lg3eekcd8o
slug: lecture7-efficient-disk-space-monitoring-with-a-shell-script
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1697822897180/04dad04a-d2bf-4af0-b034-7d2f514ffa80.png
tags: linux, devops, shell-scripting, devops-articles, masterwithhamza

---

Disk space is a precious resource on any computer system, and running out of it can lead to data loss and performance issues. To avoid such situations, it's essential to monitor available disk space regularly. In this article, we will delve into creating a shell script for disk space monitoring, helping you ensure your system maintains enough free space for smooth operation.

## **Creating a Disk Space Monitoring Script**

We'll now guide you through creating a shell script to monitor available disk space. This script checks the disk usage and alerts you when it falls below a specified threshold.

### **The Script**

```bash
#!/bin/bash

# Set the threshold (in bytes)
threshold=5000000000  # 5 GB, adjust as needed

# Get disk usage information
disk_usage=$(df -B 1 / | awk 'NR==2 {print $4}')

# Check if disk usage is below the threshold
if [ "$disk_usage" -lt "$threshold" ]; then
    echo "Warning: Low disk space! Available space is less than 5 GB."
else
    echo "Disk space is sufficient."
fi
```

### **Running the Script**

1. Save the script to a file, e.g., `disk_space_monitor.sh`.
    
2. Make the script executable with `chmod +x disk_space_monitor.sh`.
    
3. Run the script: `./disk_space_monitor.sh`.
    

![](https://miro.medium.com/v2/resize:fit:700/1*V9hEoWKjZAzBsQ2RRP6_Yg.png align="left")

## **Conclusion**

Monitoring disk space is a vital aspect of system maintenance, ensuring your computer operates smoothly and data remains safe. With the disk space monitoring script provided in this article, you can regularly check your partition's free space and receive warnings when it falls below a specified threshold. This proactive approach will help you take timely actions to address disk space issues and maintain a healthy and efficient computing environment.