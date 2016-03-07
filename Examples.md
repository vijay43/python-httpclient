
```
import httpclient

config = httpclient.Configuration()
config.set_trust_store("/path/to/verisign/ca.pem")

uri = "https://www.verisign.com/"
method = httpclient.GetMethod(uri)
method.execute()
response = method.get_response()
print "Response status: " + str(response.status)
```