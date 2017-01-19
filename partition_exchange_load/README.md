# Partition Exchange Loading

These scripts are to support Part 2 of a 3-part blog post on partition echange loading. Part 1 is here:

https://blogs.oracle.com/optimizer/entry/efficient_statistics_maintenance_for_partitioned

### [example.sql](https://github.com/oracle/dw-vldb/tree/master/partition_exchange_load/example.sql)

This script shows how partition exchange load interacts with incremental statistics for a subpartitioned main table.

### [copy_for_exchange.sql](https://github.com/oracle/dw-vldb/tree/master/partition_exchange_load/copy_for_exchange.sql)

This script demonstrates how you can copy extended statistics and histograms from a partitioned application table to a table you will be exchanging with a partition. 

### [check_hist.sql](https://github.com/oracle/dw-vldb/tree/master/partition_exchange_load/check_hist.sql)

This script checks that histograms are consistent in a partitioned table.

### Note

All of the scripts are designed to work with Oracle Database 12c.

### DISCLAIMER

*  These scripts are provided for educational purposes only.
*  They are NOT supported by Oracle World Wide Technical Support.
*  The scripts have been tested and they appear to work as intended.
*  You should always run scripts on a test instance.

### WARNING

*  These scripts drop and create tables. For use on test databases.