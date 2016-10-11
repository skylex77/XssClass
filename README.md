# XssClass
PHP Class for prevent cross-site-scripting (XSS) vulnerabilities. Removes dangerous tags and protocols from HTML.

//Call the Class<br>
$XssClass = new XssClass();

//Function Options<br>
$allowed_protocols = array('http', 'ftp', 'mailto');
$allowed_tags = array('a', 'i', 'b', 'em', 'span', 'strong', 'ul', 'ol', 'li', 'table', 'tr', 'td', 'thead', 'th', 'tbody');

//Pass the options defined before<br>
$XssClass->addAllowedProtocols($allowed_protocols);
$XssClass->addAllowedTags($allowed_tags);

//Echo the Filter<br>
echo $filtered_string = $XssClass->xss($value);
