Simply do a `git pull` then a `docker-compose up` inside the directory, and your up and running with a small infrastructure of Wordpress!

This is used to do testing for the eventual release of an automated build process on the Docker Hub. 

This will load up 1 HAProxy server, 2 Varnish server load balanced under that HAProxy server, 4 Apache Web Server backends, 1 MySQL Database server, 1 Memcached server.

Currently files need to be placed in their correct location to work after the curl above has been completed (i.e. object-cache.php in the /wp-content/ folder)

Upcoming Plans: -MariaDB Galera Cluster (3 servers) ----HyperDB -Memcached Clustering w/ mcrouter

Future Plans: -Automated build from a webhook -Full structure on git; including wordpress (future core updates will be performed in git) -Added Plugins through branches -More documentation!

...more to come soon!
