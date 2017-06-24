# Info

midPoint identity manager on Debian 9/stretch.

Homepage: [http://evolveum.com](http://evolveum.com)

Documentation: [https://wiki.evolveum.com/display/midPoint/Home](https://wiki.evolveum.com/display/midPoint/Home)

# Launch

    docker pull valtri/docker-midpoint
    docker run -itd --name midpoint valtri/docker-midpoint

# Connect

Parameters (replace the IP by real value):

* URL: **http://172.17.0.2/midpoint**
* User: **administrator**
* Password: **5ecr3t**

The IP address may be obtained:

    docker inspect -f '{{.NetworkSettings.IPAddress}}' midpoint

# Admin

    docker exec midpoint /bin/bash -l

# Tags

* **3.6-SNAPSHOT**, **latest**: midPoint 3.6