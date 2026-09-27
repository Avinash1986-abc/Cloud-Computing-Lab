# Type-1 vs Type-2 Hypervisor Comparison

## Comparison

| Parameter               | Type-1: Proxmox VE | Type-2: VMware Workstation |
| ----------------------- | ------------------ | -------------------------- |
| Hypervisor Type         | Type-1             | Type-2                     |
| Architecture            | Bare-metal         | Hosted                     |
| Guest OS                | Ubuntu             | Ubuntu                     |
| vCPU                    | 2                  | 2                          |
| Memory                  | 2 GB               | 8 GB                       |
| Disk                    | 20 GB              | 20 GB                      |
| Network                 | VirtIO / vmbr0     | NAT                        |
| Sysbench Execution Time | 10.0006 s          | 10.0003 s                  |
| Total Events            | 16903              | 17588                      |
| Events per Second       | 1689.43            | 1758.60                    |
| Minimum Latency         | 0.57 ms            | 0.55 ms                    |
| Average Latency         | 0.59 ms            | 0.57 ms                    |
| Maximum Latency         | 1.09 ms            | 1.11 ms                    |

## Performance Analysis

Both hypervisors were tested using the Sysbench CPU benchmark with a maximum prime number of 20000.

The measured results show differences in events processed per second and latency. The available memory allocation also differs between the two virtual machines, so the results should be interpreted with this configuration difference in mind.

## Conclusion

This experiment demonstrates the basic performance comparison between Type-1 and Type-2 virtualization using Ubuntu virtual machines and Sysbench CPU benchmarking.
