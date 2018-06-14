You will need to download the ebaysdk for python repository to get all the necessary files you need.

Also (not sure if it's a bug or not) but wherever you execute your script from, will need the common.py file placed there. For some reason import statement will not recognize the file unless its in current working directory.

With that said, Sandbox site isn't working because there is a bug (I'm assuming) with linking the sandbox accounts to a PayPal address. 

I tried identical script using PROD credentials, and it worked smoothly with one exception: GetTokenStatus.

u'GetTokenStatus: Class: RequestError, Severity: Error, Code: 17476, The token does not match your header credentials. The token does not match your header credentials.'
{'Ack': 'Failure', 'Timestamp': '2018-06-14T21:13:18.596Z', 'Errors': {'ErrorCode': '17476', 'LongMessage': 'The token does not match your header credentials.', 'ErrorClassification': 'RequestError', 'SeverityCode': 'Error', 'ShortMessage': 'The token does not match your header credentials.'}, 'Version': '1059', 'Build': 'E1059_CORE_APISIGNIN_18690974_R1'}

As of now this is the only error I'm having in PROD.
