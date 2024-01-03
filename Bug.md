Desciption: 

Host Header Injection is a security vulnerability that occurs when an adversary manipulates the Host
header of an HTTP request to inject or modify its value. The Host header is a part of the HTTP
request that specifies the hostname of the web server the client wants to communicate with. It is
essential for the server to properly route the request to the correct virtual host (website) if the
server is hosting multiple sites on the same IP address.

It was observed that an adversary can modify the host header value to a malicious host or domain,
allowing normal users to be redirected to a malicious website or domain while login.



4.2	Medium - A05 – Security Misconfiguration

Impact: 

By exploiting this flaw, an adversary could redirect unsuspecting normal users to fraudulent or
malicious websites during the login process. This could lead to a wide range of serious
consequences, including unauthorized access to sensitive user information, phishing attacks to steal
login credentials, or the dissemination of malware to compromise users' devices. As a result, the
trust and reputation of the targeted service or application may be severely damaged, leading to
potential financial losses, legal repercussions, and erosion of customer confidence.


It is recommended to:
 Implement strict input validation and sanitization for all user-supplied input, including the
Host header. Ensure that only valid and expected
 Maintain a whitelist of trusted hostnames that your application should interact with. Only
accept requests with Host headers that match the entries on the whitelist

Referance:

https://owasp.org/Top10/A03_2021-Injection/
https://owasp.org/www-project-web-security-testing-guide/v41/4-
Web_Application_Security_Testing/07-Input_Validation_Testing/17-Testing_for_Host_Header_Injection
