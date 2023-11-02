This ansible script will install nginx + certbot SSL cert and postfix for RPM based distros.(tested on ALMA linux)
Wend an email and the email will appear parsed to json in https://domain/new

1. almalinux role will disable selinux state.
2. nginx role will install nginx and crate basic config for SSL and list directory /new and link /var/www/new with /usr/share/nginx/new
3. smtp will configure basic smtp server to receive emails for $domain and copy the python script (https://github.com/Newsman/MailToJson).
4. After all the server will send an email to local user and the email will appear in http/s://domain/new
5. Feel free to use and edit what ever u want.

Change hosts file to add new hostname/IP and domain.
