# NPM scripts for generate self sign certificate using OpenSSL

This scripts will generate both CA certificate and Server Certificate so you can use "https" in your local development.

## How to config

You can config your domain name, IP Address in "csr.conf" and "cert.conf"

## How to Generate

```
$ npm run build
```

## Output

The script will generate output files in ./dist folder

1. rootCA.crt (import this file into your Browser, to make it trusted authority)
2. server.crt (use this file with your web server)
3. server.key (use this file with your web server)

## Example

when use with parcel dev server

```
parcel --https --cert server.crt --key server.key
```
