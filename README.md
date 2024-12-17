# Slurm Viewer

## Introduction
Using a single terminal command, slurm-viewer allows you to view the status of your SLURM cluster (i.e., nodes and jobs). This command combines information from SLURM commands like sinfo, scontrol, squeue and sacct in a tabular and customizable view.
This command line application can be run on the cluster itself or any computer that can ssh into the cluster.

## Features
- **Single command**: The `slurm-viewer` command allows you to view the status of nodes and jobs in your SLURM cluster.
  - **Multiple Clusters**: View multiple clusters in a single interface.
  - **SSH Tunneling**: Connect to the cluster using a jumphost/gateway.
- **Intuitive Interface**: `slurm-viewer` presents all node/job information in a tabular format. 
- **Customizable Interface**: Filter and sort nodes and jobs based on various criteria like partitions and GPU availability
- **Resource Utilization Plots**: View the GPU memory/utilization used over the last 4 weeks.

![slurm-viewer nodes](https://gitlab.com/lkeb/slurm_viewer/-/raw/main/assets/3__slurm-viewer__nodestatus.png "Nodes")

![Slurmviewer Queue](https://gitlab.com/lkeb/slurm_viewer/-/raw/main/assets/2__slurm-viewer__Jobs.png "Queue")

![Slurmviewer SPU](https://gitlab.com/lkeb/slurm_viewer/-/raw/main/assets/slurmviewer_gpu.svg "GPU USage")

## Installation

```bash
pip install slurm-viewer
```

If you want to test a development version, you can install it directly from the git repository:

```bash
pip install git+https://gitlab.com/lkeb/slurm_viewer.git
```
 - The code is hosted on [gitlab](https://gitlab.com/lkeb/slurm_viewer.git)
