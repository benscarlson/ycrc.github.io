# Bouchet Getting Started

The Bouchet HPC cluster is YCRC's first installation at [Massachusetts High Performance Computing Center (MGHPCC)](https://www.mghpcc.org/). 
Bouchet is the planned successor to both Grace and McCleary, with the majority of HPC infrastructure refreshes and growth deployed at MGHPCC going forward.

## Key Differences from Other Clusters

### Primary Group

On non-Bouchet clusters, your PI name is the primary group of your account. 
On Bouchet, your primary group is your NetID, and secondary groups are assigned for any PI group you belong to.
This setup makes the process of group change easier and can also accommodate 
"project"-based secondary groups rather than PI-based secondary groups.
PI groups on Bouchet take the form `pi_<netid of the pi>`, instead of `<lastname of pi>` to avoid collisions and confusion between PIs who share a lastname.    
Files created in PI-owned project and scratch directories will inherit the correct PI group-ownership.
However, be careful about copying existing files from `$HOME` to project spaces, as those files may need to have their group ownership updated.

### Partitions

For detailed information about job limits and available compute nodes in each 
partition, please refer to [our Bouchet partition documentation](/clusters/bouchet/#partitions-and-hardware). 
Please use `devel` partition for code development, debugging, and compilation. 
Jobs submitted to [`mpi` partitions](/clusters-at-yale/job-scheduling/mpi/) need to request at least two nodes and are allocated full nodes.   
The H200 GPUs are available in a dedicated partition (`gpu_h200`) and are available for all users.

### Storage

Bouchet's filesystem, Roberts, is an all-flash storage system from VAST data and does not have a GPFS filesystem. 
`/nfs/roberts/` hosts Bouchet's home, project, and scratch directories. 
Your project and scratch storage usage and quota are shared with the members of the associated secondary group.
 

|Storage         | Root Directory            | Quota                                   | File Count | 
|----------------|---------------------------|-----------------------------------------|------------|
| home           | `/nfs/roberts/home`       | 125GiB/user                             | 500,000    | 
| project        | `/nfs/roberts/project`    | 4TiB/group                              | 5,000,000  | 
| scratch        | `/nfs/roberts/scratch`    | 10TiB/group                             | 15,000,000 |


### Transfer data from other clusters

To transfer data from other clusters to Bouchet, we encourage using [Globus](/data/globus/).


### Applications and software

Commonly used software is available as [modules](/applications/modules/), similar to other clusters. 
Currently, all software is compiled and installed with the 2022b or 2024a versions of the toolchains on Bouchet, even if the same software version is installed with an older toolchain (e.g. 2020b) on other clusters.
If you would like to compile your own code specifically to the Bouchet MPI compute node architecture, you can request an interactive compute session in the `devel` partition of Bouchet. 
Because Bouchet does not have a GPFS filesystem, be sure to turn off any GPFS related optimization configuration. 


## Report Issues

If you discover issues when running your workflow or experience performance issues, feel free to [contact](/) us for assistance. 
Please include the working directory, the commands that were run, the software modules used, and any more information needed to reproduce the issue.






  
