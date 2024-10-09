#wget #recursivedownload #spider

https://www.gnu.org/software/wget/

wget can be used to recursively download the contents of a website, effectively crawling it. Beware, the content will actually be downloaded.

Example:

```
$ wget \
	--recursive \
	--page-requisites \
	--convert-links \
	--no-clobber \
	--domains <domain> \
	<url>	
```

This example gets the entire site. It can be further restricted including by depth, extension, etc.


