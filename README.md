# ZeroSSL-CertRenew
A python script that automatically renews the certificate on ZeroSSL

Change following variables:

	Line 19: Api Key
	Line 20: Domain name
	Line 43 to 52: Request paramteres (O, OU, L, ST, C)

The script assumes that certificates are stored in /etc/apache2/ssl/*.

The script assumes that the www-root is stored in /var/www/domain.com/*.

OpenSSL is used to create the private key and csr.

There is no exception handling anywhere in the code, so things might not be stable.

Execute the script with
	python3 ZeroSSL_CertRenew.py
