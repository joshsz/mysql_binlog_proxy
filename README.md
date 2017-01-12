# README driven development

* Should connect as slave to N masters, grab binlogs, and locally cache
* should give secondaries a seamless connection interface and a binlog shipping capability
* when a master dies should support promotion of a secondary to master and all other secondaries should seamlessly keep replicating without being repointed
* eventually should handle multi-master binlog merging
* should be fast and low-resource use (except for disk)

# Config

* master(s)
* binlog retention [ size | time | ? ]

# Tech

* probably should be Go just because why not? Might be spikeable in ruby or whatever
