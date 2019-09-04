---
title: nordicsmartgovernment docs
---

# nordicsmartgovernment docs

Here you will find the docs on nordicsmartgovernment and the reference implementations made by us

## Testing HOWTO

1. Install Postman (or other tool to create and execute HTTP requests) <https://www.getpostman.com/downloads/>
2. Read openAPI descriptions <https://github.com/nordicsmartgovernment/nordicsmartgovernment/tree/develop/src/main/resources/openAPI>
3. Reference implementation server URL: <https://nsg.fellesdatakatalog.brreg.no/>
4. Authorization: the reference implementation uses Basic Auth where a username and password has to be given in the request. At this moment the username and password can be anything (there are no real checks) apart from the API for submitting a voucher where the username has to be the companyId of the owner of the voucher. The companyId of the synthetic test data company is 20202020.
5. Sample requests can be downloaded from: <https://github.com/nordicsmartgovernment/nordicsmartgovernment/tree/develop/src/main/resources/SyntheticData>

### Example

A simple ping request to the Transaction API:

```
curl -i https://nsg.fellesdatakatalog.brreg.no/transactions/ping
```
