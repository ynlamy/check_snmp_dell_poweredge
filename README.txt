This plugin can check the status of Dell PowerEdge server using SNMP v1 queries and Dell OpenManage.

check_check_snmp_dell_poweredge plugin is written in Bash and is distributed under the GPLv2 license. This plugin have been created by Yoann LAMY.

Usage:
./check_snmp_dell_poweredge -H 127.0.0.1 -C public -t disk -d 1
./check_snmp_dell_poweredge -H 127.0.0.1 -C public -t fan
./check_snmp_dell_poweredge -H 127.0.0.1 -C public -t health
./check_snmp_dell_poweredge -H 127.0.0.1 -C public -t info
./check_snmp_dell_poweredge -H 127.0.0.1 -C public -t redundancy
./check_snmp_dell_poweredge -H 127.0.0.1 -C public -t temperature -w 30 -c 35

-H ADDRESS
Name or IP address of host (default: 127.0.0.1)
-C STRING
Community name for the host's SNMP agent (default: public)
-t STRING
Different status (disk, fan, health, info, power, redundancy, temperature)
-d INTEGER
Numero of disk (default: 1)
-w INTEGER
Warning level for temperature in degrees (default: 0)
-c INTEGER
Critical level for temperature in degrees (default: 0)
-h
Print this help screen
-V
Print version and license information

This plugin uses the 'snmpget' command included with the NET-SNMP package.
This plugin support performance data output.

The nagios plugins come with ABSOLUTELY NO WARRANTY.

You may redistribute copies of the plugins under the terms of the GNU General Public License v2.
