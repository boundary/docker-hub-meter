# docker-hub-meter
Contains dockerfiles and info related to TrueSight Pulse Meter containers.

To build a Docker image containing the TrueSight Pulse Meter, clone this repo, cd into the directory, and run the following command:

*sudo docker build -t `<name[:tag]>` --build-arg METER_PACKAGE_VER=`<meter version>` -f dockerfile.ubuntu-trusty .*

e.g.  *sudo docker build -t mymeter --build-arg METER_PACKAGE_VER=4.2.4-661 -f dockerfile.ubuntu-trusty .*

If you'd like to create a Docker image that will monitor host level metrics from a containerized meter, use the same command above with the dockerfile-host-metrics.ubuntu-trusty dockerfile.

e.g.  *sudo docker build -t mymeter --build-arg METER_PACKAGE_VER=4.2.4-661 -f dockerfile-host-metrics.ubuntu-trusty .*

You can locate the latest available version of the meter by checking the current production repo: [http://apt.boundary.com/#!/ubuntu/pool/universe/b/boundary-meter/](http://apt.boundary.com/#!/ubuntu/pool/universe/b/boundary-meter/)

For more information on the TrueSight Pulse Meter container image for Docker, please visit: [https://hub.docker.com/r/bmctruesightpulse/meter](https://hub.docker.com/r/bmctruesightpulse/meter)
