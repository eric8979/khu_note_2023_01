- web application << web site
	- "web site running web-application"

- The big picture (pg.3)

- apache, nginx -> repsond for static info requests(html, css ..)


### Directory listing
- Was a functionality
- Accessing un-authorized dirs.

### Local File Inclusion
- Adding `?page=../../../../../WINDOWS/system32/drivers` behind url
	- GET request param

### .htaccess
- quite old vuln

### Upload vulnerability
- Upload 
	- e.g. adding file to an email
- Hiding real extension
	- e.g. `backdoor.php.png`
- Uploading/getting the "web-shell"

### **Web-shell**
- A Program injected by attacker after penetration succeeds. 
- Permanent backdoor
- Often built using PHP.

### SQL injection

### XSS
- HTML/JS code injection
- Injecting JS code into a website for other users to execute it.
	- Vuln for where users communicate.
- Circumvent SOP(Same-Origin-Policy)
- Insert malicious JS to be executed from users.

### CSRF

### http & https
- https = http + SSL/TLS
- new : `ftp://blabla`

# 3.27~
### http
- GET
	- data/param in url
- POST
	- data in Header
 
### Header
- Variables
	- Host
		- For virtual servers
	- User-Agent
		- device info, browser info
	- Referer
		- Contains address from which a source has been requested.
	- Cookie
		- Identify a user

### Web firewall

## 3.29~
### Base64
- Not all ascii char is visible, therefore base64 for text based use-cases.
	- e.g. encoding video or text with ascii might include something like `http GET` but with base64 there is no `space` which is important for http protocol.
	- url query string doesn't use spacebar, `+` instead.
		- and % for hexadecimal (more than just alphabet) pg.44
- `echo -n 'encoded_string' | base64 -d`


### Bind shell

### Reverse shell

### Server-Side Template Injection
- SSTI
- Even if the vuln is not critical, it could be used for **fingerprinting**.

### SOP
- Prevents one server's script accessing properties of a different server.
- Stopping attacks using `<frame>` of authentic website inside of malicious website.

### AJAX
- AJAX allows web pages to be updated asynchronously by exchanging data with a web server behind the scenes.
- with JSON