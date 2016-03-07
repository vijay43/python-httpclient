This project aims to provide an HTTP client library for Python to address some of the shortcomings of httplib and urllib2, in particular:
  * verification of SSL certificates,
  * usage of client certificate authentication with SSL,
  * SSL connections through a proxy,
  * usage of methods other than GET and POST.

**Please note that this project is not maintained.** Despite some efforts to improve the state of certificate verification, there are probably shortcomings in this project in this area (or others). You can of course have a look at the code, but you should certainly consider using an alternative library, since bugs will not be fixed in this project, and no guarantee is made regarding its correctness.