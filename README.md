# MySQL NDB Cluster 8.0.26 "cluster-in-a-box" setup

This repository contains the original configuration files used in the blog post "Scale-up MySQL NDB Cluster 8.0.26 to +1.5M QPS the easy way with AMD EPYC 7742"
([Medium](https://tiagomlalves.medium.com/scale-up-mysql-ndb-cluster-8-0-26-to-1-5m-qps-the-easy-way-with-amd-epyc-7742-3e2e42a6bd0) | [MySQL Blogs](https://dev.mysql.com/blog-archive/scale-up-mysql-ndb-cluster-8-0-26-to-1-5m-qps/) | [AMD Performance Brief](https://www.amd.com/content/dam/amd/en/documents/epyc-business-docs/performance-briefs/amd-epyc-7002-pb-mysql-ndb-cluster-qps.pdf)).

Files are:
 * config.ini - MySQL NDB Management Node configuration file
 * my.cnf - MySQL Server configuration file

These configurations were tailored for the following server specifications:
 * 1x Dell EMC PowerEdge R7525 server, configured with
 * Dual processor AMD Epyc 7742 (ROME), 64-core processor, 128 threads, 7nm design, max clock speed 3900MHZ, and 256MB cache
 * 32x 64GB DDR4 dimms (SK Hynix), 3200 MT/s (total 2TB of RAM)
 * 4x 3.2TB NVMe drives (Dell Express Flash PM1725b)

Configurations were used to demo how to setup a high-performance single-box cluster in a simple way using MySQL NDB Cluster 8.0.26.
