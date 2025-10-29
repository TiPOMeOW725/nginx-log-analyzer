# Nginx Log Analyzer
## Description
A simple shell script to analyze nginx access logs and extract statistics about IP addresses, requested paths, response codes, and user agents.
## Prerequisites
- Bash shell
- Standard Unix utilities: awk, sed, grep, sort, uniq, tail
- An nginx access log file
## Installation
Clone this repository or download the script:
```
git clone <your-repo-url>
cd nginx-log-analyzer
```
Make the script executable:
```
chmod +x nginx-log-analyzer
```
## Usage
Run the script with the path to your nginx log file as an argument:

```
./nginx-log-analyzer /path/to/nginx-access.log
```

## Sample Output
```
Top 5 IP addresses with the most requests:
45.76.135.253 - 1000 requests
142.93.143.8 - 600 requests
178.128.94.113 - 50 requests
43.224.43.187 - 30 requests
178.128.94.113 - 20 requests
---

Top 5 most requested paths:
/api/v1/users - 1000 requests
/api/v1/products - 600 requests
/api/v1/orders - 50 requests
/api/v1/payments - 30 requests
/api/v1/reviews - 20 requests
---

Top 5 response status codes:
200 - 1000 requests
404 - 600 requests
500 - 50 requests
401 - 30 requests
304 - 20 requests
---

Top 5 user agents:
Mozilla/5.0... - 1000 requests
curl/7.64.1 - 600 requests
...
```
