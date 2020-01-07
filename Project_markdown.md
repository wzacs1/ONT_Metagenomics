Date 20-01-06

W. Zac Stephenss

# Background
Process:
1. Base call (optional, would usually do locally with Guppy)
2. Clean reads. QC/nanopolish
3. Remove human mapping reads, mouse mapping reads (later, check both of these against microbial)
4. Assembly-based metagenomes
5.


# Method
1. Build container with
   1. Guppy
   2. nanopolish
   3. SqueezeMeta

# Container building
Would like to build a single container with multiple metagenomics tools for sake of simplicity in sharing with lab. 

### Installing SqueezeMeta
Just clone repository on github in container. However, for database, pull them outside of container building. Much too big. Then use the noDB perl script in SqueezeMEta
#### Database
Clone SqueezeMeta and use perl script (or just copy script only from git) to get databases in common location
perl scripts/preparing_databases/download_databases.pl ~/round-group1/reference_seq_dbs/SqueezeMeta/


# Input Files
1. Reference database?
2.

``` {r}
get.
```
#
