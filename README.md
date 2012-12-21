# Rddclient 

Rddclient is a tiny DynDNSClient based on ruby. Due to my modem (Fritz
7390) which does not support multiple hostnames, this script was
created to fit my needs. Works with dyndns.org only. Just look at the file
and adjust some settings.

## Install

Just make sure to have all required stuff using ruby-gems. Copy the script to your
  load-path and make it executable.
  
Then adjust these settinge to fit your hostnames and emailsettings for
  notifying:
  ```
  @@username="test"
  @@password="test"
  @@hostnames=[
               "test.ath.cx",
               "test.dnsalias.net",
               "test.dnsalias.org",
               "test.homeip.net",
               "test.merseine.nu"
              ]
              
  @@checkInterval = 300  # seconds                                                                                                                                                                                                                                                                                                                                                                
  @@logIpPath  = "/var/log/dyndns.log"
  
  # Mail settings                                                                                                                                                                                      
  @@toalias="Me"
  @@subject="[DYNDNS]"
  @@from="server@example.com"
  @@to="me@example.com"
  ```
* **Start with following args:**

```
  -d daemon to run in background
  -t terminal to run in foreground
  -h to show this help text

```
