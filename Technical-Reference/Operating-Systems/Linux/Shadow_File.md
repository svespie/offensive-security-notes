[Understanding /etc/shadow file format on Linux - nixCraft (cyberciti.biz)](https://www.cyberciti.biz/faq/understanding-etcshadow-file/)

![](../../../_attachments/etc_shadow.png)

Requires elevated privileges to access it often contains password hashes.

Colon separated fields as with /etc/passwd.

The fields:

| kali                                                                        | username in plaintext                                     |
| --------------------------------------------------------------------------- | --------------------------------------------------------- |
| `$y$j9T$OJdvOD2KWRcv3jwj/qVtl1$K4p5stod.MsiigDRmKJu0miVFptvTNCIx7cGKBGO7P6` | encrypted password; `$y$` indicates the hashing algorithm |
| 19794                                                                       | timestamp indicating last password change                 |
| 0                                                                           | minimum number of days before required password reset     |
| 99999                                                                       | maximum number of days the password is valid for          |
| 7                                                                           | number of days prior to expiration to notify user         |



![](../../../_attachments/yescrypt.png)

`$ man 5 crypt`
