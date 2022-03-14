# LFI - Local File Include

## Summary

File inclusions are crucial for any server-side scripting languages and are responsible for content of files to be used as of an app’s code. Local File Inclusion (LFI) occurs when malicious actors trick a web app into either running or exposing files on a web server, potentially causing sensitive information such as passwords or API keys to leak.

* Without properly implemented filtering, an attacker can request a specific path of a file and get access to sensitive information
* An attacker can attempt to inject malicious input to server log files and gain remote code execution 
* Exploiting the LFI vulnerability can lead to code execution on the client-side and lead to further attacks, such as cross-site scripting (XSS) 

## Detection
* Detecting LFI is most easily done with an automated vulnerability scanner as it’s a widespread vulnerability
* [Code scans](https://brightsec.com/blog/local-file-inclusion-lfi/#manually-testing-for-lfi) can be performed in order to detect LFI weaknesses before hitting production servers

## Solution
- [x] Implement proper filtering making sure no other than the intended files can be accessed.

## Further Reading
* <https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-21804>
* <https://www.acunetix.com/blog/articles/local-file-inclusion-lfi/>
* <https://owasp.org/www-project-web-security-testing-guide/v41/4Web_Application_Security_Testing/07-Input_Validation_Testing/11.1-Testing_for_Local_File_Inclusion>
