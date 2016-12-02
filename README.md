# Docker Scripts

###### A series of small docker scripts to do specific activity in various docker images

## Overview

A general repo of a series of scripts used in my docker images to get specific tasks accomplished. 

## Scripts

#### `ha-transmission-client.sh`

 - Bounces transmission and vpn connection.
 - Openvpn's implementation seems to not flush the route table after a soft device restart [source needed] and many vpn providers provide randomized ip addresing when restarting so the route table needs to reflect the new gateways. Bouncing the entire connection (a hard device reset if you will) will accomplish this and, while not a fix, is a cheap workaround. 
