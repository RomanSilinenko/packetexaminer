# packetexaminer
----
This is a somple harness to do PCAP analysis. This hopefully automates a lot of the function an analyst would do manually. 

Coming in the next day or two is visualization using NetworkX

#Features
----
It currently supports:
*Counts of IPs
*Bytes between IPS
*DNS lookups
*URLs


#Usage
----
    [joe@fedora26 packetexaminer]$ ./packetexaminer.py --help | sed 's/^/     /'
     usage: packetexaminer.py [-h] [--flows] [--dst] [--src] [--bytes] [--dns]
                              [--url] [--all] [--limit LIMIT]
                              file
     
     PCAP File Examiner
     
     positional arguments:
       file           Source PCAP File, i.e. example.pcap
     
     optional arguments:
       -h, --help     show this help message and exit
       --flows        Display flow summary
       --dst          Display count of destination IPs
       --src          Display count of source IPs
       --bytes        Display source and destination byte counts
       --dns          Display all DNS Lookups in PCAP
       --url          Display all ULRs in PCAP
       --all          Display all
       --limit LIMIT  Limit results to X
