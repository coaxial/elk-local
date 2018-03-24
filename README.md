# Local ELK

This is the configuration I am using for my internal ELK setup.

Probably not too useful to anyone else as is, but good for inspiration or comparing notes.

Make sure the virtual memory limit is high enough. More info:
https://www.elastic.co/guide/en/elasticsearch/reference/5.0/vm-max-map-count.html#vm-max-map-count.
TLDR: `$ sysctl -w vm.max_map_count=262144 # command to execute
on the Linux docker host`

Copy the example env files and change the variables to what is appropriate.

Run it all with `$ docker-compose up -d && docker-compose logs -f`
