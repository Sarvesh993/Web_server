# Developing a Simple Webserver
## AIM:

To develop a simple webserver to serve html pages.
## DESIGN STEPS:
### Step 1:

HTML content creation
### Step 2:

Design of webserver workflow
### Step 3:

Implementation using Python code
### Step 4:

Serving the HTML pages.
### Step 5:

Testing the webserver
## PROGRAM:
<!DOCTYPE html>
<html>
<head>
<title>My webserver</title>
</head>
<body>
<h1>p.sarveshvaran</h1>
<h2>krishsarveshvaran18@gmail.com></h2>
<h3>21004775</h3>
</body>
</html>
"""
class myhandler(BaseHTTPRequestHandler):
    def do_GET(self):
        print("request received")
        self.send_response(200)
        self.send_header('content-type', 'text/html; charset=utf-8')
        self.end_headers()
        self.wfile.write(content.encode())
server_address = ('',1001)
httpd = HTTPServer(server_address,myhandler)
print("my webserver is running...")
httpd.serve_forever()
~

## OUTPUT:
![GitHub Logo](xyz.png)
## RESULT:
webserver is created succesfully

## OUTPUT:
## RESULT:
