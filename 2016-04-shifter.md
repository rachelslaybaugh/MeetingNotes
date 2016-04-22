2016-04-21
----------

#### shifter HPC meeting

- Cori stats; working on improving connectivity; have user defined images for
  complex workflows
- for data intensive software stacks--for people who want to install lots of
  software and use all of it ("big software") 100s MB to GB
- docker-like functionality
- needing more and more data intensive processing across doe facilities
- goal: create images with certified stacks for software projects with specific
  stack requirements
- Let the user construct the image they care about and use that
- have a hookup system that will enable use of the local exotic features of the
  hardware (interconnect, etc.)
- make docker container and host on dockerhub (which is sharable...not sure if
  we can do that).
- "don't want staff adding latency to user's work"
- shifter adds mount points, home directory, (rewrite etc), and so on to make
  things work, so it will not completely be your image. 
- this way you can use parallel file service, etc. want integrated into batch
  system. 
- when you're on the supercomputer you're you, not root. You make the image as
  root, but have to set up with the knowledge you cannot be root later.
- can't directly use docker for a variety of reasons, so they use docker as a
  basis but make their own thing
- use ChOS (kernel manager that deals with chroots (chroot changes from the
  root that you know about, but what looks like the root directory
  changes--facilitates the appearance of a different OS, can change libc, etc.))
- Shifter supports Docker images, CHOS images, and other image types
- file permissions are maintained, but who owns what doesn't matter
- (what does stripe image across multiple OSTs mean?)
- very tunable way to distribute images
- CLI, have an image gateway that does the DockerHub interaction and creates
  and stores images on lustre, handles path merging stuff so that the paths
  make sense for your image
- "no one should set an LD_LIBRARY_PATH in their container", just install your
  software
- overwrite a bunch of stuff that won't be needed; make sure to follow
  directions about where to install stuff or not to avoid path conflicts once
  on the machine; shouldn't be too hard
- (pynamic python benchmark) (squashfs)
- shifter on par with local memory
- NO CURRENT ABILITY TO PROTECT IMAGE FROM OTHER PEOPLE USING IT (future
  release plan; we cannot use it until that happens...)
- can ssh into another node and land in the container
- 
