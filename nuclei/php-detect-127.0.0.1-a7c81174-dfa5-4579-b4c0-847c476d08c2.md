### PHP Detect (php-detect) found on 127.0.0.1

----
**Details**: **php-detect** matched at 127.0.0.1

**Protocol**: HTTP

**Full URL**: http://127.0.0.1:4280

**Timestamp**: Wed Nov 18 14:28:36 +0100 CET 2026

**Template Information**

| Key | Value |
| --- | --- |
| Name | PHP Detect |
| Authors | y0no |
| Tags | tech, php, discovery |
| Severity | info |
| CVSS-Score | 0.00 |
| vendor | php |
| product | php |
| shodan-query | X-Powered-By: PHP |

**Request**
```http
GET / HTTP/1.1
Host: 127.0.0.1:4280
User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_6) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/15.2 Safari/605.1.15
Cookie: ***
Accept-Encoding: gzip


```

**Response**
```http
HTTP/1.1 200 OK
Cache-Control: no-cache, must-revalidate
Content-Type: text/html;charset=utf-8
Date: Wed, 18 Nov 2026 13:28:36 GMT
Expires: Tue, 23 Jun 2009 12:00:00 GMT
Pragma: no-cache
Server: Apache/2.4.69 (Debian)
Vary: Accept-Encoding
X-Powered-By: PHP/8.5.12

<!DOCTYPE html>

<html lang="en-GB">

	<head>
		<meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />

		<title>Welcome :: Damn Vulnerable Web Application (DVWA)</title>

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
				<ul class="menuBlocks"><li class="selected"><a href=".">Home</a></li>
<li class=""><a href="instructions.php">Instructions</a></li>
<li class=""><a href="setup.php">Setup / Reset DB</a></li>
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
	<h1>Welcome to Damn Vulnerable Web Application!</h1>
	<p>Damn Vulnerable Web Application (DVWA) is a PHP/MySQL web application that is damn vulnerable. Its main goal is to be an aid for security professionals to test their skills and tools in a legal environment, help web developers better understand the processes of securing web applications and to aid both students & teachers to learn about web application security in a controlled class room environment.</p>
	<p>The aim of DVWA is to <em>practice some of the most common web vulnerabilities</em>, with <em>various levels of difficultly</em>, with a simple straightforward interface.</p>
	<hr />
	<br />

	<h2>General Instructions</h2>
	<p>It is up to the user how they approach DVWA. Either by working through every module at a fixed level, or selecting any module and working up to reach the highest level they can before moving onto the next one. There is not a fixed object to complete a module; however users should feel that they have successfully exploited the system as best as they possible could by using that particular vulnerability.</p>
	<p>Please note, there are <em>both documented and undocumented vulnerabilities</em> with this software. This is intentional. You are encouraged to try and discover as many issues as possible.</p>
	<p>There is a help button at the bottom of each page, which allows you to view hints & tips for that vulnerability. There are also additional links for further background reading, which relates to that security issue.</p>
	<hr />
	<br />

	<h2>WARNING!</h2>
	<p>Damn Vulnerable Web Application is damn vulnerable! <em>Do not upload it to your hosting provider's public html folder or any Internet facing servers</em>, as they will be compromised. It is recommend using a virtual machine (such as <a href="https://www.virtualbox.org/" target="_blank">VirtualBox</a> or <a href="https://www.vmware.com/" target="_blank">VMware</a>), which is set to NAT networking mode. Inside a guest machine, you can download and install <a href="https://www.apachefriends.org/" target="_blank">XAMPP</a> for the web serv.... Truncated ....
```

**Extra Information**

**Extracted results:**

- 8.5.12



**CURL command**
```sh
curl -X 'GET' -d '' -H 'Cookie: ***' -H 'Host: 127.0.0.1:4280' -H 'User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_6) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/15.2 Safari/605.1.15' 'http://127.0.0.1:4280'
```

----

Generated by [Nuclei v3.11.1](https://github.com/projectdiscovery/nuclei)