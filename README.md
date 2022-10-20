### Certificate Bundle Generator

This script will generate a Certificate Bundle from a Server Certificate that was created by the TAK Server CA Scripts.
It will output a PEM formatted Server Certificate, Private Key and a Certificate Authority Bundle that contains your Root and Intermediate CA.

These can be used in other services such as OpenFire, Apache etc..

Usage: ./certBundleGen {domain} {certificate}

{domain} The Fully Qualified Domain Name for your server. This can actually be anything you want. However, using the FQDN makes it easy to identify what the bundle is for.
{certificate} The PCKS12 formatted Server Certificate that is located in your /opt/tak/certs/files directory.

Example: ./certBundleGen emfour.local xmppserver.p12
