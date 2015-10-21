O2CURL
=====
[O2CURL][3] is an Open Source PHP Lightweight HTTP Request Client Libraries. 
Another amazing product from [PT. Lingkar Kreasi (Circle Creative)][1], released under MIT License.
[O2CURL][3] is build for working more powerfull with O2System Framework, but also can be used for integrated with others as standalone version with limited features.
[O2CURL][3] is insipired by [Unirest][10], so [O2CURL][2] is has also functionality similar with it, but a little bit different at the syntax.

Features
--------
- Utility methods to call GET, HEAD, POST, PUT, DELETE, CONNECT, OPTIONS, TRACE, PATCH requests
- Supports form parameters, file uploads and custom body entities
- Supports gzip
- Supports Basic, Digest, Negotiate, NTLM Authentication natively
- Customizable timeout
- Customizable default headers for every request (DRY)
- Automatic JSON parsing into a native object for JSON responses

Installation
------------
The best way to install O2CURL is to use [Composer][9]
```
composer require o2system/o2curl:'dev-master'
```

Usage
-----
```
$headers = array("Accept" => "application/json");
$content = array("foo" => "hello", "bar" => "world");

$curl = new \O2System\CURL;
$response = $curl->post("http://domain.com/", 'request/json', $headers, $content);

$response->meta;        // HTTP Request Metadata
$response->headers;     // Headers
$response->body;        // Parsed body
$response->raw_body;    // Unparsed body
```

More details at the Wiki. (Coming Soon)

Ideas and Suggestions
---------------------
Please kindly mail us at [developer@o2system.in][7].

Bugs and Issues
---------------
Please kindly submit your [issues at Github][5] so we can track all the issues along development.

System Requirements
-------------------
- PHP 5.4+
- Composer

Credits
-------
* Founder and Lead Projects: [Steeven Andrian Salim (steevenz.com)][7]

[1]: http://circle-creative.com
[2]: http://o2system.in
[3]: http://o2system.in/features/standalone/o2cache
[4]: http://o2system.in/features/standalone/o2cache/license
[5]: http://github.com/circlecreative/o2cache/issues
[6]: https://packagist.org/packages/o2system/o2cache
[7]: http://steevenz.com
[8]: mailto:developer@o2system.in
[9]: https://getcomposer.org
[10]: http://unirest.io
