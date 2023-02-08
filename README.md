# DEVNET-2459
Examples from Cisco Live EMEA 2023



# cisco_live.py
This script should be saved to /etc/netbox/scripts. 
This path can be changed by setting SCRIPTS_ROOT in NetBox's configuration. 

1. Creates a Netbox Form - collects input data in netbox (site code, name, number of switches)
2. Creates new site
3. Selects next available IP prefix, reserves it for the site
4. DNS reservations for router and switches
5. Creates rack
6. Creates devices
7. Assigns IPs to interfaces
8. Adds devices to NSO and fetches their ssh host keys


# configure_dhcp_with_netbox.py
This script we can run from the environment, where NSO is running

1. Gets the information on site subnet from Netbox,
2. Reserves new pool in Netbox for site DHCP server
3. Configures router as DHCP server
