# http_check_2 - a simple nagios http check script

## Usage

```bash
user$ bin/check_http_2 -h
This is a simple nagios check script for checking the http status.

Syntax: check_http_2 [[[-u url ] [-s status-code] [-t check-content]] | [-h]]
options:
-u | --url            Adds the url you want to check.
-p | --path           The path you want to check (default is "/").
-s | --status-code    The expected status code.
-t | --content        The content the request must contain.

-h | --help           Shows this help dialog.
-v | --version        Shows the version of this script.
```

```bash
user$ bin/check_http_2 -u https://www.futuresax.de -p /unternehmen -s 200 -t "<title>futureSAX für Unternehmen | futureSAX</title>"
HTTP OK: HTTP/1.1 200 OK - 70900 bytes in 0.683 second response time
```
