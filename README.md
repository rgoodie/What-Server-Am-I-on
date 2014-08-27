What
----
Appends the server name to the browser title bar. Useful if editing a Drupal installation that sites on a load balancer with a primary production and a secondary fail over production boxes joined with one-way database replication.

Why
----
If your load balancer fails over to another production server and your database replication is one-way, how do content editors know on which server they are currently editing? Will changes be lost once the infrastructure switches back over to the primary server and database? 

How
----
- Clone the repo into /sites/all/modules/, 
- Enable the module
- Name the production and failover server hostnames* [ /admin/config/soc/wsaio ] 



Errata and footnotes
------
* You can find your hostname by typing `hostname` directly into your terminal (mac, linux, or windows using cygwin)


