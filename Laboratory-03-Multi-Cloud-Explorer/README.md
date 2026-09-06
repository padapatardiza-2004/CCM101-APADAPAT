# Mission 3 – Multi-Cloud Explorer

## Checkpoint 7 – Exploring a Linux Environment with KillerCoda

For this checkpoint, a Linux-based environment was examined through KillerCoda. Several standard Linux commands were executed to gather important system details such as the operating system, processor, memory usage, and disk capacity.

---

## 1. Checking the Operating System

To determine which Linux distribution and version were running in the environment, the following command was executed:

```bash
cat /etc/os-release
```

This command reads the `os-release` file, which contains identifying information about the installed Linux distribution, including its name and version.

### Terminal Evidence 1 – OS Details

![KillerCoda Terminal 1 - OS Details](screenshots/killercoda-terminal-1.png)

---

## 2. Examining the CPU

The processor configuration was examined using:

```bash
lscpu
```

The output provides technical information about the CPU, such as the processor architecture, CPU count, and other processor-related specifications.

### Terminal Evidence 2 – CPU Details

![KillerCoda Terminal 2 - CPU Details](screenshots/killercoda-terminal-2.png)

---

## 3. Checking Memory Usage

To view the system's memory allocation and availability, this command was used:

```bash
free -h
```

The `-h` option presents the memory values in an easier-to-read format. The results include the total, currently used, free, and available memory.

### Terminal Evidence 3 – Memory Details

![KillerCoda Terminal 3 - Memory Details](screenshots/killercoda-terminal-3.png)

---

## 4. Checking Disk Capacity

The storage space of the Linux environment was checked using:

```bash
df -h
```

This command reports information about the mounted file systems, including their total capacity, used space, remaining space, and percentage of utilization.

### Terminal Evidence 4 – Disk Details

![KillerCoda Terminal 4 - Disk Details](screenshots/killercoda-terminal-4.png)

---

## System Investigation Summary

| Information Checked | Linux Command         | Evidence            |
| ------------------- | --------------------- | ------------------- |
| Operating System    | `cat /etc/os-release` | Terminal Evidence 1 |
| Processor           | `lscpu`               | Terminal Evidence 2 |
| Memory              | `free -h`             | Terminal Evidence 3 |
| Storage             | `df -h`               | Terminal Evidence 4 |

The commands above provide a quick way for a system administrator to inspect the main components and resources of a Linux machine.

---

## Possible Cloud Migration

A Linux server running in a local or virtual environment can also be deployed to a cloud platform. Major cloud providers offer virtual machine services capable of running Linux operating systems.

| Cloud Platform            | Virtual Machine Service |
| ------------------------- | ----------------------- |
| Amazon Web Services (AWS) | Amazon EC2              |
| Microsoft Azure           | Azure Virtual Machines  |
| Google Cloud              | Compute Engine          |

These services allow organizations to run Linux servers in cloud-based virtual machines without maintaining the physical server infrastructure themselves.

---


