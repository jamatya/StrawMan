# Remove harmful tags from the content

Validation Service uses HTML Santizer which has been configured to remove the following harmful tags
- script
- iframe
- object
- embed

It can be further configured to 
- allow specific tags and attributes and ignore the rest
- allow specific url schemes (http, https, mailto, tel) and ignore rest 
- remove attributes that might be dangerous such as onclick, prevent inline js in links
- to custom handle specific tags etc.

The content includes a bunch of html code including script and iframe tags, which should be removed in the sanitized markdown file.
<b> Be careful of these tags! </b>
<script>alert("Run me!")</script>
<iframe>dslfsdjflksdfdsf</iframe>

<i>can you see these tags?</i>
