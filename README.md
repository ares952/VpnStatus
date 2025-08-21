# VpnStatus
Provides VPN status of connected devices with the history of all connections

## Configuration
* database connection has to be configured for nette
* cron job must be installed or systemd service must be enabled to update the state regularly
* path to openvpn log folder must be configured (that one where openvpn.log  openvpn-status.log are updated)
  
## Overview
* provides the current status of connected devices
* provides the current logs for last N lines
* provides the history of connected devices
* provides the history logs for last Y lines

## Security
User must ensure that the status is stored on local network  not to be accessible from outside or the website is after the reverse proxy with e.g. cookie configured.
