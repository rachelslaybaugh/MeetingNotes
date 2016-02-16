Cloud Computing meeting

### <a name="top">Index
[CFN Cluster, 2016/02/11](#2016-02-11)


#### <a name="2016-02-11"> CFN cluster, 2016.01.11

(get slides; I showed up about 35 minutes late)
- any EC2 size is allowed, can have head node and compute nodes be different
  sizes
- schedulers: slurm, sge, openlava, or torque
- can use a bunch of linux options: ubuntu is one of them
- CFN cluster cookbook
- persistent storage available via EBS-volume
- temporary storage as scratch with ephemeral disks
- autoscaling parameters
- autoshutdown available
- keychain for storing credentials securely
- configure stuff; make sure the subnet you choose can connect to your vpc
- r series is better if you need more memory than comput power
 
[Index](#top)
