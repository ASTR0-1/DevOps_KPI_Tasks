# Docker build:
docker build . -t hwforlection5

# Docker run with memory and cpu restriction:
docker run -p 41690:80 -m 100m --cpus="2"  -d hwforlection5

# Test node.js server:
curl -i localhost:41690

# Ouput exapmle:
HTTP/1.1 200 OK
X-Powered-By: Express
Content-Type: text/html; charset=utf-8
Content-Length: 11
ETag: W/"b-Ck1VqNd45QIvq3AZd8XYQLvEhtA"
Date: Mon, 31 Oct 2022 12:34:35 GMT
Connection: keep-alive
Keep-Alive: timeout=5

Hello World