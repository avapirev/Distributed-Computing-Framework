# Distributed-Computing-Framework
Framework for deploying Hadoop and Spark on a shared cluster within a batch job.

The official repository is hosted on Bitbucket [here](https://bitbucket.org/avapirev/distributed-computing-framework/src/master/).

What is DCF
===========

DCF stands for Distributed data Computing cluster Framework. It is a collection of bash scripts which configure and launch a Hadoop and/or Spark clusters within a batch job (pbs, slurm, sge) on a traditional shared HPC cluster. The current version has been tested on Apache Hadoop 3.2.1 and Spark 3. The various scripts parse through the job environment to define certain Hadoop/Spark requirements, e.g., list of the job hostnames necessary to fire up the clusters. The default configuration assures minimal working environment with respect to the batch job settings. Further Hadoop/Spark cluster parameter configuration and optimization is left to the user. That can be automatically passed down with a flag pointing to the location where the customized config files are. The contents of the latter will be added to the already determined minimal framework configuration.

Released under GNU General Public License v2.

Requirements
============

* Bash 4 or newer
* The GNU getopt for parsing short and long option names (by default on most Linux systems).
* Java
* Hadoop and/or Spark
* User configuration input (optional)
* Python 3 (optional)

Usage
=====

See the [User Guide](https://bitbucket.org/avapirev/distributed-computing-framework/src/master/USERGUIDE.md).
