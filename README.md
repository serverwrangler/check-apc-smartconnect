# check-apc-smartconnect
Pull data from the APC smartconnect cloud app, allowing for ingest into icinga

This can be run using `./apc-smartconnect.pl <ups-id> <email> <password>`

The ups-id is shown in the url when using smartconnect.apc.com/.
#pre-reqs
 - Ubuntu/debian
 `sudo apt install libwww-perl`
 - Redhat/Centos
 `sudo yum install perl-libwww-perl` 
 - OSX
 `sudo perl -MCPAN -e ‘install Bundle::LWP’`
 
