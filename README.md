# DirectEditWithPython
This is a script for using Let's Encrypt's DNS-01 with MyDNS.JP.

Unlike [DirectEdit](https://github.com/disco-v8/DirectEdit), it uses Python instead of PHP for updates.

## Usage

### When running for the first time

 1. Edit `regist_dns01.sh`. The edited part is as follows.
	```
	id=<Your MyDNS.JP ID>
	pwd=<Your MyDNS.JP Password>
	domain=<Your Domain>
	email=<Your E-mail>
	hook_script=<Absolute path to "dns01.py">
	```
 2. Run `regist_dns01.sh`.

### After the second time

 1. Run `certbot renew`.

