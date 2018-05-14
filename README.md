# nginx-docker
A simple docker rep to serve as load balancer and api gateway.
i.e.
For development, if you want to put client rendering service and api service in the same machine, this can drive the traffic to different upstream, and avoid CORS issue.

For ubuntu
Use --net="host" in docker run command to allow docker container to access your upstream in host.

For mac, use `host.docker.internal` instead of `localhost` in nginx conf.