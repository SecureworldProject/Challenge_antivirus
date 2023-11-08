# Challenge_antivirus
Challenge that generates a different key depending on the number of installed AVs.

It requires `pip install windows-tools.antivirus`


ejemplo de configuracion json
```json
{
	"FileName": "antivirus_challenge.dll",
	"Description": "Challenge that generates a different key depending on the number of installed AVs.",
	"Props": {
		"validity_time": 3600,
		"refresh_time": 3000
	},
	"Requirements": "none"
}

```
