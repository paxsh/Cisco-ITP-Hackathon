# Cisco-ITP-Hackathon
Malicious URL Checker

The malicious URL detector was made as a part of the Cisco ITP Hackathon in 2018.

This code uses the awesome MITM proxy library, which can be found here: https://github.com/mitmproxy/mitmproxy/
and Cisco's umbrella api to get "threat-scores" on the URL's. A negative or "-1" value indicates maliciousness. The docs for Cisco's Umbrella API can be found here: https://docs.umbrella.com/developer/investigate-api/

Running this script with the mitm proxy will check for "maliciousness" in the URL's one's about to visit and redirect to a web page hosted on your own web server in an event of a malicious URL.

Running the script:
./mitmproxy -s /path/to/the/script
