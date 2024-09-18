#google #googlehacking #googledorking

Search engines can be useful for information gathering by crawling and indexing information about a given target and resources through creative searches.

Many of these techniques apply to other search engines, as well. Do not be afraid to review the respective documentation for variances.

[Refine Google searches - Google Search Help](https://support.google.com/websearch/answer/2466433?hl=en)

Some pre-defined and oddly specific Google search queries can be found here: [Google Hacking Database (GHDB) - Google Dorks, OSINT, Recon (exploit-db.com)](https://www.exploit-db.com/google-hacking-database).

Here are some basic operators:

| **Operator**           | **Description**                                   | **Example**                                    | **Purpose**                                  |
|------------------------|---------------------------------------------------|------------------------------------------------|----------------------------------------------|
| `site:`                | Restrict results to a specific site or domain.    | `site:example.com`<br>Find all indexed pages for `example.com`. | Find all indexed pages for a specific site or domain.    |
| `inurl:`               | Find pages with a specific keyword in the URL.    | `inurl:admin`<br>Locate pages with "admin" in the URL. | Locate pages with a specific keyword in the URL.        |
| `intitle:`             | Search for pages with a keyword in the title.     | `intitle:login`<br>Find pages with "login" in the title. | Search for pages with a keyword in the title.        |
| `intext:`              | Search for pages containing specific text.        | `intext:"confidential"`<br>Locate pages with "confidential" in the content. | Locate pages containing specific text in the content. |
| `filetype:`            | Find files of a specific type.                    | `filetype:pdf site:example.com`<br>Search for PDF files on `example.com`. | Search for files of a specific type on a site.       |
| `cache:`               | View Google's cached version of a page.           | `cache:example.com`<br>See the cached version of `example.com`. | View Google's cached version of a page.     |
| `link:`                | Find pages that link to a specific URL.           | `link:example.com`<br>Discover pages linking to `example.com`. | Find pages that link to a specific URL.     |
| `related:`             | Find sites related to a specific site.            | `related:example.com`<br>Identify sites related to `example.com`. | Identify sites related to a specific site.     |
| `allintitle:`          | Search for pages with all specified words in the title. | `allintitle:secure login`<br>Locate pages with "secure" and "login" in the title. | Locate pages with multiple keywords in the title. |
| `allinurl:`            | Find pages with all specified words in the URL.   | `allinurl:login.php`<br>Locate URLs containing "login.php". | Find pages with multiple keywords in the URL.          |
| `allintext:`           | Search for pages with all specified words in the text. | `allintext:password reset`<br>Find pages containing "password reset" in the content. | Search for pages with multiple keywords in the text. |
| `*` (Asterisk)         | Use as a wildcard to match any word(s).           | `"password * 123"`<br>Find phrases like "password for 123". | Use as a wildcard in searches.        |
| `OR`                   | Search for results containing either term.        | `admin OR login`<br>Locate pages containing "admin" or "login". | Search for results containing either term.  |
| `-` (Minus)            | Exclude pages containing the specified term.      | `site:example.com -inurl:login`<br>Find pages on `example.com` excluding URLs with "login". | Exclude pages containing the specified term. |
| `"` (Quotes)           | Search for an exact phrase.                       | `"admin panel"`<br>Locate pages with the exact phrase "admin panel". | Search for an exact phrase. |
| `define:`              | Find definitions of words.                        | `define:phishing`<br>Get the definition of "phishing". | Find definitions of words.            |
| `numrange:`            | Search for a range of numbers.                    | `numrange:2000-2020`<br>Find results containing numbers between 2000 and 2020. | Search for a range of numbers. |
| `before:` and `after:` | Find pages published before or after a date.      | `site:example.com before:2020`<br>Locate pages on `example.com` published before 2020. | Find pages published before or after a date. |
| `info:`                | Get information about a URL.                      | `info:example.com`<br>Show information about `example.com`. | Get information about a URL.        |
| `inanchor:`            | Search for pages with specified anchor text.      | `inanchor:"click here"`<br>Find pages with anchor text "click here". | Search for pages with specific anchor text.    |
| `AROUND(X)`            | Find pages where terms are within X words of each other. | `security AROUND(3) update`<br>Locate pages where "security" is near "update". | Find pages where terms are within X words of each other. |




![](Google_Hacking_BlackHat.pdf)