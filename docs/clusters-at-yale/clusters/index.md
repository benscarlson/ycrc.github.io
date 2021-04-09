# HPC Resources

## Compute

We maintain and support four compute clusters, listed below. Please click on cluster names for more information. To download a Word document that describes our facilities, equipment, and other resources for HPC and research computing, click [here](https://research.computing.yale.edu/sites/default/files/files/Facilities%20and%20Equipment%20Document-2020-02-27.docx).

| Cluster Name       | Approx. Core Count | Approx. Node Count | Login Address<img width=200/> | Purpose                                                  |
|--------------------|--------------------|---------------------|-------------------------------|----------------------------------------------------------|
| [Grace](grace)     | 24,000             | 850                 | `grace.hpc.yale.edu`          | general and highly parallel, tightly coupled             |
| [Farnam](farnam)   | 5,700              | 250                 | `farnam.hpc.yale.edu`         | medical/life science                                     |
| [Ruddle](ruddle)   | 3,200              | 200                 | `ruddle.hpc.yale.edu`         | [Yale Center for Genome Analysis](http://ycga.yale.edu/) |
| [Milgram](milgram) | 2,400              | 80                  | `milgram.hpc.yale.edu`        | HIPAA/sensitive data                                     |

## Storage

We maintain several high performance storage systems which amount to about 12.5 PiB total. Listed below are these shared filesystems and the clusters where they are available. We distinguish where clusters store their home directories with an asterisk. The directory `/home` will always point to your home directory on the cluster you logged into. For more information about storage quotas and purchasing storage see the [Cluster Storage](/clusters-at-yale/data/index) page.

| Filesystem    | Size    | Mounting Clusters     |
|---------------|---------|-----------------------|
| /gpfs/gibbs   | 4.1 PiB | Grace, Farnam, Ruddle |
| /gpfs/loomis  | 2.6 PiB | Grace\*, Farnam       |
| /gpfs/ysm     | 1.5 PiB | Grace, Farnam\*       |
| /gpfs/slayman | 1.0 PiB | Grace, Farnam         |
| /gpfs/ycga    | 2.0 PiB | Ruddle\*              |
| /gpfs/milgram | 1.1 PiB | Milgram\*             |
