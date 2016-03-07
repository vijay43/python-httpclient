# Introduction #

This httpclient library aims to address shortcomings of urllib2, included in
the core Python (2.4/2.5) distribution, mainly:
  * its handling of proxy servers (especially HTTPS),
  * its handling of SSL/TLS certificate (lack of verification),
  * other HTTP methods (PUT, ...).


# Requirements #

This library will try to use Python's [ssl module](http://docs.python.org/library/ssl.html), if available (Python 2.6). Otherwise, it will require the [PyOpenSSL library](http://pyopenssl.sourceforge.net/).

Please check the [Features](Features.md) page for differences of feature and implementation.


# Design #

The design of these classes is loosely based on the [Apache HttpClient library (Java)](http://hc.apache.org/httpclient-3.x/).