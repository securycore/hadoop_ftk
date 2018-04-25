# Hadoop File System Forensics Toolkit (HDFS FTK)
View and extract files from an offline image of Hadoop file system.


### Motivation
In Hadoop File Systems, metadata such as filename, access time and file system hierachy information is stored in the namenode. The actual data is stored in the datanodes in _blocks_. Although HDFS has command client tools to manage the extraction files, it only works with a running cluster of HDFS machines.
This python script aims to provide investigators with the ability to perform forensics analysis of offline evidence captures of Hadoop File System images.

## Instructions

### PreRequisites
* Python 3.x
* PrettyTable: `pip install prettytable`

### Usage

```
Hadoop Forensics File System Forensics Tool Kit (HDFS FTK) ver. 1.0
usage: hdfs_ftk.py [-h] [-v] [-d D] [-o O] -f F

HDFS Forensics Toolkit.

optional arguments:
  -h, --help       show this help message and exit
  -v, --verbose    Verbose mode
  -d D             Number of Datanodes
  -o O, -output O  output directory

Required named arguments:
  -f F             Path to fsimage

```

#### Example commands:

To view contents of HDFS File System: `python hdfs_ftk.py -f fsimage.xml`
```