# Features and status #

## SSL client certificates ##

It is possible to authenticate via a client certificate:

```
config = Configuration()
config.set_client_cert("/path/to/client-cert.pem")
config.set_client_key("/path/to/client-cert.key")
```

## SSL verification ##

This code requires the server to present a certificate. This certificate is verified against trust anchors (a concatenation of CA certificates in PEM format).

```
config.set_trust_store("/path/to/ca-concat.pem")
```

| **Feature/Library used** | **2.6/ssl** | **PyOpenSSL** |
|:-------------------------|:------------|:--------------|
| Hostname matches CN field of subject DN | Yes         | Yes           |
| Hostname matches subjectAltName DNS | Yes         | Not yet       |