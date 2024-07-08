# building a debian12 based singularity/apptainer container for scipion3 (using cuda 12.3 which is the oldest cuda version for debian12 as of 2024/07/08)

Tru <tru@pasteur.fr>

## Why ?
- ready to use runtime environment for scipion3
- just add miniconda and scipion3 (use a writable bind mount for /opt)
- allow easy snapshoting/replacement for /opt and upgrade/downgrade
- share scipion with your co-worker

## How to:
- build the container
- use the container with a mounted /opt to
	- install miniconda and scipion-installer
	- install any plugin/binary
- use mksquashfs "freeze" your scipion and share it with the debian runtime

## References
- https://scipion.i2pc.es/

## Caveat
- playground, use at your own risk!
