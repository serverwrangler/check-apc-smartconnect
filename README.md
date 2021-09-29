# check-apc-smartconnect
Pull data from the APC smartconnect cloud app, allowing for ingest into icinga

This can be run using `./apc-smartconnect.pl <ups-id> <email> <password>`

The ups-id is shown in the url when using smartconnect.apc.com/.
# pre-reqs

## libwww-perl
 - Ubuntu/debian
 `sudo apt install libwww-perl`
 - Redhat/Centos
 `sudo yum install perl-libwww-perl` 
 - OSX
 `sudo perl -MCPAN -e ‘install Bundle::LWP’`


 ## JSON
- `brew install cpanm`
- `sudo cpanm install JSON`


## APC SmartConnect API Endpoint urls
This url returns many parameters from the ups (Battery, input, output, outlets, and network status)
- `https://smartconnect.apc.com/api/v1/gateways/<MAC ADDRESS OF APC UPS>?collection=input,output,battery,network,main_outlet,switched_outlets`

This url returns model information, firmware version, check-in status, warranty status,and ups name/description
- `https://smartconnect.apc.com/api/v1/gateways/<MAC ADDRESS OF APC UPS>/`
