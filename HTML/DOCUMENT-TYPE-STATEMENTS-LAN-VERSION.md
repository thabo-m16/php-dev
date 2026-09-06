Document Type Statements and Language Versions
(X)HTML documents should begin with a <!DOCTYPE> declaration. This statement
identifies the type of markup that is supposedly used in a document. For example,
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN">
indicates that we are using the transitional variation of HTML 4.01 that starts with a root
element html. In other words, an <html> tag will serve as the ultimate parent of all the
content and elements within this document.
A <!DOCTYPE> declaration might get a bit more specific and specify the URI (Uniform
Resource Identifier) of the DTD being used as shown here:
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN"
"http://www.w3.org/TR/html4/loose.dtd">
In the case of an XHTML document, the situation really isn’t much different:
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
However, do note that the root html element here is lowercase, which hints at the case
sensitivity found in XHTML.

HTML or XHTML Version !DOCTYPE Declaration
HTML 2.0 <!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML//EN">
HTML 3.2 <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 3.2 Final//EN">
HTML 4.0 Transitional <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0 Transitional//EN"
"http://www.w3.org/TR/html4/loose.dtd">
HTML 4.0 Frameset <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0 Frameset//EN"
"http://www.w3.org/TR/html4/frameset.dtd">
HTML 4.0 Strict <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0//EN"
"http://www.w3.org/TR/html4/strict.dtd">
HTML 4.01 Transitional <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN"
"http://www.w3.org/TR/html4/loose.dtd">
HTML 4.01 Frameset <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Frameset//EN"
"http://www.w3.org/TR/html4/frameset.dtd">
HTML 4.01 Strict <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN"
"http://www.w3.org/TR/html4/strict.dtd">
HTML5 <!DOCTYPE html>
XHTML 1.0 Transitional <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
XHTML 1.0 Strict <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
XHTML 1.0 Frameset <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Frameset//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-frameset.dtd">
XHTML 1.1 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN"
"http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">
XHTML 2.0 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 2.0//EN"
"http://www.w3.org/MarkUp/DTD/xhtml2.dtd">
XHTML Basic 1.0 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML Basic 1.0//EN"
"http://www.w3.org/TR/xhtml-basic/xhtml-basic10.dtd">
XHTML Basic 1.1 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML Basic 1.1//EN"
"http://www.w3.org/TR/xhtml-basic/xhtml-basic11.dtd">

Alternatively, in either HTML or XHTML (but not in HTML5), we can replace the
<body> tag with a <frameset> tag, which encloses potentially numerous <frame> tags
corresponding to individual portions of the browser window, termed frames. Each frame in
turn would reference another HTML/XHTML document containing either a standard
document, complete with <html>, <head>, and <body> tags, or perhaps yet another
framed document. The <frameset> tag also should include a noframes element that
provides a version of the page for browsers that do not support frames. Within this element, a <body> tag should be found for browsers that do not support frames.

To set the appropriate character set, you should include a <meta> tag before the page title even though traditionally title is considered the first element.

