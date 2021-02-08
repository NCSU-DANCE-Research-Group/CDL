# CDL: Classified Distributed Learning for Detecting Security Attacks in Containerized Applications

This contains the data of our [paper](https://doi.org/10.1145/3427228.3427236). If you find this data useful in your research, please consider citing:

	@inproceedings{lin2020cdl,
	title={CDL: Classified Distributed Learning for Detecting Security Attacks in Containerized Applications},
	author={Lin, Yuhang and Tunde-Onadele, Olufogorehan and Gu, Xiaohui},
	booktitle={Annual Computer Security Applications Conference},
	pages={179--188},
	year={2020},
	publisher = {Association for Computing Machinery},
	series = {ACSAC '20}
	}

## System Calls Frequency Vectors
We collected the system call data from 33 real-world vulnerabilities where each line represents the frequencies every 0.1 second interval.

The list of 33 vulnerabilites are listed below:
| Threat Impact                            | CVE ID         | CVSS | Score                     | Application Version |
|------------------------------------------|----------------|------|---------------------------|---------------------|
| Return a shell and execute arbitrary code | CVE-2012-1823  | 7.5  | PHP                       | 5.4.1               |
|                                          | CVE-2014-3120  | 6.8  | Elasticsearch             | 1.1.1               |
|                                          | CVE-2015-1427  | 7.5  | Elasticsearch             | 1.4.2               |
|                                          | CVE-2015-2208  | 7.5  | phpMoAdmin                | 1.1.2               |
|                                          | CVE-2015-3306  | 10   | ProFTPd                   | 1.3.5               |
|                                          | CVE-2015-8103  | 7.5  | JBoss                     | 6.1.0               |
|                                          | CVE-2016-3088  | 7.5  | Apache ActiveMQ           | 5.11.1              |
|                                          | CVE-2016-9920  | 6    | Roundcube                 | 1.2.2               |
|                                          | CVE-2016-10033 | 7.5  | PHPMailer                 | 5.2.16              |
|                                          | CVE-2017-7494  | 10   | Samba                     | 4.5.9               |
|                                          | CVE-2017-8291  | 6.8  | Ghostscript               | 9.2.1               |
|                                          | CVE-2017-11610 | 9    | Supervisor                | 3.3.2               |
|                                          | CVE-2017-12149 | 7.5  | JBoss                     | 6.1.0               |
|                                          | CVE-2017-12615 | 6.8  | Apache Tomcat             | 8.5.19              |
| Execute arbitrary code                   | CVE-2014-6271  | 10   | Bash                      | 4.2.37              |
|                                          | CVE-2015-8562  | 7.5  | Joomla                    | 3.4.2               |
|                                          | CVE-2016-3714  | 10   | ImageMagick               | 6.7.9               |
|                                          | CVE-2017-5638  | 10   | Apache Struts 2           | 2.5                 |
|                                          | CVE-2017-12794 | 4.3  | Django                    | 1.11.4              |
|                                          | CVE-2018-16509 | 9.3  | Ghostscript               | 9.23                |
|                                          | CVE-2018-19475 | 6.8  | Ghostscript               | 9.25                |
|                                          | CVE-2019-6116  | 6.8  | Ghostscript               | 9.26                |
| Disclose credential information          | CVE-2014-0160  | 5    | OpenSSL                   | 1.0.1e              |
|                                          | CVE-2015-5531  | 5    | Elasticsearch             | 1.6.0               |
|                                          | CVE-2017-7529  | 5    | Nginx                     | 1.13.2-1            |
|                                          | CVE-2017-8917  | 7.5  | Joomla                    | 3.7.0               |
|                                          | CVE-2018-15473 | 5    | OpenSSH                   | 7.7p1               |
|                                          | CVE-2020-1938  | 7.5  | Apache Tomcat             | 9.0.30              |
| Consume excessive CPU                    | CVE-2014-0050  | 7.5  | Apache Commons FileUpload | 1.3.1               |
|                                          | CVE-2016-6515  | 7.8  | OpenSSH                   | 7.2p2               |
| Crash the application                    | CVE-2015-5477  | 7.8  | BIND                      | 9                   |
|                                          | CVE-2016-7434  | 5    | NTP                       | 1.4.2.8             |
| Escalate privilege level                 | CVE-2017-12635 | 10   | CouchDB                   | 2.1.0               |


## File Naming Convention
We collected seven minute traces in four separate containers for each CVE. In each CVE directory, you can find four files. The files with names ending in "full" are the full frequency vectors of a container.  

## Update Since Publication
1/2021: Container 4 of CVE-2019-6116 has wrong timing information thus we replaced it.  
