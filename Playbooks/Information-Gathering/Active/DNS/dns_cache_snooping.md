#dns

[http://blog.commandlinekungfu.com/2009/03/episode-17-dns-cache-snooping-in-single.html](http://blog.commandlinekungfu.com/2009/03/episode-17-dns-cache-snooping-in-single.html)

If we query DNS with recursion turned off from a compromised host, it may be possible to ascertain information about the environment just by determining what domains users on the network are visiting.

This is done by setting the Recursion Desired (RD) bit to 0 in the DNS request.


Tools:
[nslookup](../../../../Tools/nslookup/non-recursive_search.md)
[dig](../../../../Tools/dig/non-recursive_search.md)


