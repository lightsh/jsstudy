﻿TODO 01
========

* 아래 코드를 복사/붙여넣기 내공을 사용하십시오.
* message 버튼을 클릭하세요.
* C'est fini.

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<meta charset="UTF-8">
		<style type="text/css">
		
			table, th, td {
				border: 1px solid gray;
				border-collapse: collapse;
			}
			
			th, td {
				padding: 15px;
			}
			
			
		</style>
		<script type="text/javascript">
			
				
			var Base64 = {

				// private property
				_keyStr : "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/=",

				// public method for encoding
				encode : function (input) {
					var output = "";
					var chr1, chr2, chr3, enc1, enc2, enc3, enc4;
					var i = 0;

					input = Base64._utf8_encode(input);

					while (i < input.length) {

						chr1 = input.charCodeAt(i++);
						chr2 = input.charCodeAt(i++);
						chr3 = input.charCodeAt(i++);

						enc1 = chr1 >> 2;
						enc2 = ((chr1 & 3) << 4) | (chr2 >> 4);
						enc3 = ((chr2 & 15) << 2) | (chr3 >> 6);
						enc4 = chr3 & 63;

						if (isNaN(chr2)) {
							enc3 = enc4 = 64;
						} else if (isNaN(chr3)) {
							enc4 = 64;
						}

						output = output +
						this._keyStr.charAt(enc1) + this._keyStr.charAt(enc2) +
						this._keyStr.charAt(enc3) + this._keyStr.charAt(enc4);

					}

					return output;
				},

				// public method for decoding
				decode : function (input) {
					var output = "";
					var chr1, chr2, chr3;
					var enc1, enc2, enc3, enc4;
					var i = 0;

					input = input.replace(/[^A-Za-z0-9\+\/\=]/g, "");

					while (i < input.length) {

						enc1 = this._keyStr.indexOf(input.charAt(i++));
						enc2 = this._keyStr.indexOf(input.charAt(i++));
						enc3 = this._keyStr.indexOf(input.charAt(i++));
						enc4 = this._keyStr.indexOf(input.charAt(i++));

						chr1 = (enc1 << 2) | (enc2 >> 4);
						chr2 = ((enc2 & 15) << 4) | (enc3 >> 2);
						chr3 = ((enc3 & 3) << 6) | enc4;

						output = output + String.fromCharCode(chr1);

						if (enc3 != 64) {
							output = output + String.fromCharCode(chr2);
						}
						if (enc4 != 64) {
							output = output + String.fromCharCode(chr3);
						}

					}

					output = Base64._utf8_decode(output);

					return output;

				},

				// private method for UTF-8 encoding
				_utf8_encode : function (string) {
					string = string.replace(/\r\n/g,"\n");
					var utftext = "";

					for (var n = 0; n < string.length; n++) {

						var c = string.charCodeAt(n);

						if (c < 128) {
							utftext += String.fromCharCode(c);
						}
						else if((c > 127) && (c < 2048)) {
							utftext += String.fromCharCode((c >> 6) | 192);
							utftext += String.fromCharCode((c & 63) | 128);
						}
						else {
							utftext += String.fromCharCode((c >> 12) | 224);
							utftext += String.fromCharCode(((c >> 6) & 63) | 128);
							utftext += String.fromCharCode((c & 63) | 128);
						}

					}

					return utftext;
				},

				// private method for UTF-8 decoding
				_utf8_decode : function (utftext) {
					var string = "";
					var i = 0;
					var c = c1 = c2 = 0;

					while ( i < utftext.length ) {

						c = utftext.charCodeAt(i);

						if (c < 128) {
							string += String.fromCharCode(c);
							i++;
						}
						else if((c > 191) && (c < 224)) {
							c2 = utftext.charCodeAt(i+1);
							string += String.fromCharCode(((c & 31) << 6) | (c2 & 63));
							i += 2;
						}
						else {
							c2 = utftext.charCodeAt(i+1);
							c3 = utftext.charCodeAt(i+2);
							string += String.fromCharCode(((c & 15) << 12) | ((c2 & 63) << 6) | (c3 & 63));
							i += 3;
						}

					}

					return string;
				}

			}

			
			window.onload = function() {
				document.getElementById("message").onclick = function() {					
					alert(Base64.decode("MjAxNOuFhCDtlZwg7ZW0IOqzoOyDne2VmOyFqOyKteuLiOuLpC4K64K064WE7JeUIOuNlCDsl7Tsi6ztnogg7ZW07IScIOyekOuwlOyKpO2BrOumve2KuCDsoJXrs7Ug7ZWp7Iuc64ukLgrqsJDtnogg64Ko7JeQ6rKMIOuztOyXrOyjvOq4sCDsqr0g7YyU66awIO2XiOygke2VnCDsvZTrk5zripQg7J207KCcIOq3uOunjCwg7ZKI6rKpIOyeiOuKlCDsvZTrk5zroZwg64u564u57ZW07KeA6ri4LgoKTCdlZmZvcnQgZXN0IG1hIGZvcmNlLCBtYWlzIGplIG5lIHZldXggcGFzIHRyYXZhaWxsZXIuLi4uIF4uKg=="));
				}
			}
				
		</script>
	</head>
<body>
<input type="button" value="message" id="message"/>
</body>
</html>

```
