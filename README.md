ebay.yaml has configuration files that are needed to access Sandbox and PROD eBay environments. All current testing is being done on Sandbox.

ebay5.py is a direct copy of https://github.com/timotheus/ebaysdk-python/blob/master/samples/trading.py, except with the init_options function filled out ebay.yaml values.

The other change to the file is I added 'domain=...' to all of the api=Trading() functions. If there is a way for you to change this and put it into init_options, that would be great :-)

I think most of the functions are working -- other than AddItems which keeps asking for me to crete a seller account (which I already have).
