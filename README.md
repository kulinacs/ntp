ntp
===


What is does this role do?
--------------------------

This role installs and configures the openntp daemon to synchronize the system clock.


Meta
----

Files Managed:
  * /etc/ntpd.conf
  * /etc/iptables.d/ntp.rules
  * /var/service/ntpd

Defaults Provided:
  * ntp_servers: [{0,1,2,3}.pool.ntp.org]

Variables Required:
  * ntp_servers: List of servers to synchronize from

Optional Variables:
  * None

Files Required:
  * None

Optional Files:
  * None

Conflicting Roles:
  * None

Depends On:
  * [network](https://github.com/void-ansible-roles/network)
