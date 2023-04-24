# blog-EEEE
Vulnerability Title:jfinal_cms there is XSS

Affected versions:jfinal cms v5.1.0

Date of discovery: April 24, 2023

Found by: Shenwei

Analysis report: In the background, system administration, user management, adding users, there are stored XSS vulnerabilities, entering <script>alert ('xss')</script> in logins, real names, etc. will be stored in the database

Patching scheme: To save the database content, you need to filter, set filter, filter <>'" and other symbols
