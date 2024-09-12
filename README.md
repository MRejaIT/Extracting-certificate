# Extracting-certificate-
Extracting the certificate and keys from a .pfx

#Run the poweshell run as administrator
cd "C:\Program Files\Git\usr\bin\"

#Run the following command to extract the private key
.\openssl.exe pkcs12 -in [yourfile.pfx] -nocerts -out [drlive.key]

#Run the following command to decrypt the private key:
.\openssl rsa -in [drlive.key] -out [drlive-decrypted.key]

#Run the following command to extract the certificate
.\openssl.exe pkcs12 -in [yourfile.pfx] -clcerts -nokeys -out [drlive.crt]
