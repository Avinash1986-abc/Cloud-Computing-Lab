
# Experiment 1 – Virtualization Performance Analysis

## Objective

To study and analyze the performance of virtual machines using Type-1 and Type-2 hypervisors and compare their CPU performance using Sysbench.

## Overview

This experiment explores two approaches to virtualization:

* **Type-1 Hypervisor:** Proxmox VE, which runs directly on physical hardware.
* **Type-2 Hypervisor:** VMware Workstation, which runs on top of a host operating system.

Ubuntu virtual machines are configured on both platforms. System resources are verified using Linux commands, and CPU performance is measured using the Sysbench benchmarking tool.

## Experiment Structure

### Part A – Type-1 Hypervisor: Proxmox VE

Proxmox VE is used to create and run an Ubuntu virtual machine using a bare-metal virtualization environment.

**Covered activities:**

* Virtual machine creation and configuration
* Ubuntu installation
* CPU, memory, and disk verification
* System monitoring
* Sysbench CPU benchmarking
* Recording performance results

### Part B – Type-2 Hypervisor: VMware Workstation

VMware Workstation is used to create and run an Ubuntu virtual machine on a host operating system.

**Covered activities:**

* Virtual machine creation and configuration
* Ubuntu installation
* CPU, memory, and disk verification
* System monitoring
* Sysbench CPU benchmarking
* Recording performance results

### Part C – Performance Comparison

The results obtained from both virtualization environments are compared using common performance metrics.

**Comparison parameters:**

* CPU configuration
* Memory allocation
* Disk allocation
* Total execution time
* Total events
* Events per second
* Minimum latency
* Average latency
* Maximum latency

## Tools and Technologies

| Tool / Technology  | Purpose                            |
| ------------------ | ---------------------------------- |
| Proxmox VE         | Type-1 virtualization              |
| VMware Workstation | Type-2 virtualization              |
| Ubuntu             | Guest operating system             |
| Sysbench           | CPU performance benchmarking       |
| Linux Terminal     | System verification and monitoring |

## Linux Commands Used

```bash
hostnamectl
lscpu
free -h
df -h
top
```

### Sysbench CPU Benchmark

```bash
sysbench cpu --cpu-max-prime=20000 run
```


## Result

The virtual machines were successfully configured and tested using the selected hypervisors. CPU performance was measured using Sysbench and the obtained results were recorded for comparison.

## Conclusion

This experiment provides practical knowledge of virtualization, hypervisor architecture, virtual machine resource allocation, system monitoring, and performance benchmarking.
