# phpinfo disclosure

## Summary

The phpinfo(); function will emit the full php configuration of the server including all version numbers of all installed modules. Some applications include a phpinfo.php by default.![Image title](https://i.yt.gl/get/44ecc/ixoolpoghy50.png){ align=right, width="300" }

* The phpinfo(); function leaks the php version and version of all installed modules
* The phpinfo(); function can leak credentials and other sensitive information, including server environment variables
* Knowing the file system structure might give an attacker an advantage, especially if your site is vulnerable to directory traversal attacks


## Solution
- [x] In most cases, the best solution is to remove the affected file. 

## Further Reading
* <https://www.php.net/manual/en/function.phpinfo.php>
* <https://stackoverflow.com/questions/3196011/what-security-problems-could-come-from-exposing-phpinfo-to-end-users>

