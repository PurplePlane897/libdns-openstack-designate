# OpenStack Designate for `libdns`

[![godoc reference](https://img.shields.io/badge/godoc-reference-blue.svg)](https://pkg.go.dev/github.com/libdns/openstack)


This package implements the libdns interfaces for the [OpenStack Designate API](https://docs.openstack.org/api-ref/dns/) (using the Go implementation from: github.com/gophercloud/gophercloud/openstack)

## Authenticating

To authenticate you need to supply a OpenStack API credentials and zone name on which you want to operate.

## Credentials needed to authenticate to the OpenStack Designate API
```bash
 OS_REGION_NAME=""
 OS_AUTH_URL=""
 OS_AUTH_TYPE="" # Should be v3applicationcredential
 OS_APPLICATION_CREDENTIAL_ID=""
 OS_APPLICATION_CREDENTIAL_SECRET=""
```
## Example

You can find minimal example of how to get all your DNS records using this `libdns` provider in examples directory (see `examples/main.go`)