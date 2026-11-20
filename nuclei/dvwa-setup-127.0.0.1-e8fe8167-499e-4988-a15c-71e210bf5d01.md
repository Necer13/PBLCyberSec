### DVWA Exposed Setup Page (dvwa-setup) found on 127.0.0.1

----
**Details**: **dvwa-setup** matched at 127.0.0.1

**Protocol**: HTTP

**Full URL**: http://127.0.0.1:4280/setup.php

**Timestamp**: Wed Nov 18 14:30:10 +0100 CET 2026

**Template Information**

| Key | Value |
| --- | --- |
| Name | DVWA Exposed Setup Page |
| Authors | mayoubmalik1-blip |
| Tags | dvwa, setup, misconfig, vuln |
| Severity | high |
| Description | A Damn Vulnerable Web Application (DVWA) setup page is exposed. An unauthenticated attacker can use the setup page to reset the database, which restores the default credentials (admin:password), and the page discloses database configuration details. |
| shodan-query | title:dvwa |

**Request**
```http
GET /setup.php HTTP/1.1
Host: 127.0.0.1:4280
User-Agent: Mozilla/5.0 (Windows NT 6.3; Win64; x64; rv:109.0) Gecko/20100101 Firefox/116.0
Accept: */*
Accept-Language: en
Cookie: ***
Accept-Encoding: gzip


```

**Response**
```http
HTTP/1.1 200 OK
Cache-Control: no-cache, must-revalidate
Content-Type: text/html;charset=utf-8
Date: Wed, 18 Nov 2026 13:30:10 GMT
Expires: Tue, 23 Jun 2009 12:00:00 GMT
Pragma: no-cache
Server: Apache/2.4.69 (Debian)
Vary: Accept-Encoding
X-Powered-By: PHP/8.5.12

<!DOCTYPE html>

<html lang="en-GB">

	<head>
		<meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />

		<title>Setup :: Damn Vulnerable Web Application (DVWA)</title>

		<link rel="stylesheet" type="text/css" href="dvwa/css/main.css" />

		<link rel="icon" type="\\image/ico" href="favicon.ico" />

		<script type="text/javascript" src="dvwa/js/dvwaPage.js"></script>

	</head>

	<body class="home light">
		<div id="container">

			<div id="header">

				<img src="dvwa/images/logo.png" alt="Damn Vulnerable Web Application" />
                <a href="#" onclick="javascript:toggleTheme();" class="theme-icon" title="Toggle theme between light and dark.">
                    <img src="dvwa/images/theme-light-dark.png" alt="Damn Vulnerable Web Application" />
                </a>
			</div>

			<div id="main_menu">

				<div id="main_menu_padded">
				<ul class="menuBlocks"><li class=""><a href=".">Home</a></li>
<li class=""><a href="instructions.php">Instructions</a></li>
<li class="selected"><a href="setup.php">Setup / Reset DB</a></li>
</ul><ul class="menuBlocks"><li class=""><a href="vulnerabilities/brute/">Brute Force</a></li>
<li class=""><a href="vulnerabilities/exec/">Command Injection</a></li>
<li class=""><a href="vulnerabilities/csrf/">CSRF</a></li>
<li class=""><a href="vulnerabilities/fi/.?page=include.php">File Inclusion</a></li>
<li class=""><a href="vulnerabilities/upload/">File Upload</a></li>
<li class=""><a href="vulnerabilities/captcha/">Insecure CAPTCHA</a></li>
<li class=""><a href="vulnerabilities/sqli/">SQL Injection</a></li>
<li class=""><a href="vulnerabilities/sqli_blind/">SQL Injection (Blind)</a></li>
<li class=""><a href="vulnerabilities/weak_id/">Weak Session IDs</a></li>
<li class=""><a href="vulnerabilities/xss_d/">XSS (DOM)</a></li>
<li class=""><a href="vulnerabilities/xss_r/">XSS (Reflected)</a></li>
<li class=""><a href="vulnerabilities/xss_s/">XSS (Stored)</a></li>
<li class=""><a href="vulnerabilities/csp/">CSP Bypass</a></li>
<li class=""><a href="vulnerabilities/javascript/">JavaScript Attacks</a></li>
<li class=""><a href="vulnerabilities/authbypass/">Authorisation Bypass</a></li>
<li class=""><a href="vulnerabilities/open_redirect/">Open HTTP Redirect</a></li>
<li class=""><a href="vulnerabilities/cryptography/">Cryptography</a></li>
<li class=""><a href="vulnerabilities/api/">API</a></li>
</ul><ul class="menuBlocks"><li class=""><a href="security.php">DVWA Security</a></li>
<li class=""><a href="phpinfo.php">PHP Info</a></li>
<li class=""><a href="about.php">About</a></li>
</ul><ul class="menuBlocks"><li class=""><a href="logout.php">Logout</a></li>
</ul>
				</div>

			</div>

			<div id="main_body">

				
<div class="body_padded">
	<h1>Database Setup <img src="dvwa/images/spanner.png" /></h1>

	<p>Click on the 'Create / Reset Database' button below to create or reset your database.<br />
	If you get an error make sure you have the correct user credentials in: <em>/var/www/html/config/config.inc.php</em></p>

	<p>If the database already exists, <em>it will be cleared and the data will be reset</em>.<br />
	You can also use this to reset the administrator credentials ("<em>admin</em> // <em>password</em>") at any stage.</p>
	<hr />
	<br />

	<h2>Setup Check</h2>

	<em>General</em><br />
	Operating system: <em>*nix</em><br />
	<br>
	DVWA version: <em>Unknown</em><br><br>
	<br>
	reCAPTCHA key: <span class="failure">Missing</span><br />
	<br />
	Writable folder /var/www/html/hackable/uploads/: <span class="success">Yes</span><br />
	Writable folder /var/www/html/config: <span class="success">Yes</span>
	<br />
	<br>

	<em>Apache</em><br>
	Web Server SERVER_NAME: <em>127.0.0.1</em><br /><br>
	mod_rewrite: <em><span class='success'>Enabled</span></em><br>
	mod_rewrite is required for the API labs.<br><br>

	<em>PHP</em><br>
	PHP version: <em>8.5.12</em><br />
	
	PHP function display_errors: <span class="success">Enabled</span><br />
	PHP function display_startup_errors: <span class="success">Enabled</span><br />
	PHP function allow_url_include: <span class="success">Enabled</span> - Feature deprecated in PHP 7.4, see lab for more information<br/ >
	PHP function allow_url_fopen: <span class="success">Enabled</span><br />
	PHP module gd: <span class="success">Installed</span><br />
	PHP module mysql: <span class="success">Installed</span><br />
	PHP module pdo_mysql: <span class="success">Installed</span><br />
	<br />
	<em>Database</em><br>
	Backend database: <em>MySQL/MariaDB</em><br />
	Database username: <em>dvwa</em><br />
	Database password: <em>******</em><br />
	Database database: <em>dvwa</em><br />
	Database host: <em>db</em><br />
	Database port: <em>3306</em><br />
	<br />
	<em>API</em><br>
	<i>This section is only important if you want to use the .... Truncated ....
```

References: 
- https://github.com/digininja/DVWA

**CURL command**
```sh
curl -X 'GET' -d '' -H 'Accept: */*' -H 'Accept-Language: en' -H 'Cookie: ***' -H 'User-Agent: Mozilla/5.0 (Windows NT 6.3; Win64; x64; rv:109.0) Gecko/20100101 Firefox/116.0' 'http://127.0.0.1:4280/setup.php'
```

----

Generated by [Nuclei v3.11.1](https://github.com/projectdiscovery/nuclei)