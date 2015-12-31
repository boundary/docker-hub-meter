# docker-hub-meter
Contains dockerfiles and info related to TrueSight Pulse Meter containers (*STAGING/PRE-RELEASE*).

To build a Docker image containing a TrueSight Pulse Meter from the *STAGING* repository, clone this repo, cd into the directory, and run the following command:

*sudo docker build -t `<name[:tag]>` --build-arg METER_PACKAGE_VER=`<meter version>` -f dockerfile.ubuntu-trusty .*

e.g.  *sudo docker build -t mymeter --build-arg METER_PACKAGE_VER=4.2.3-639 -f dockerfile.ubuntu-trusty .*

You can locate the latest available *STAGING* version of the meter by checking the current *STAGING* repo: [http://apt-staging.boundary.com/#!/ubuntu/pool/universe/b/boundary-meter/](http://apt-staging.boundary.com/#!/ubuntu/pool/universe/b/boundary-meter/)

For more information on the TrueSight Pulse Meter container image for Docker, please visit: [https://hub.docker.com/r/bmctruesightpulse/meter-staging](https://hub.docker.com/r/bmctruesightpulse/meter-staging)
