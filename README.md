# Challenge_antivirus
Challenge que genera una clave diferente en función del número de antivirus instalados.

Requiere instalar la librería apropiada con `pip install windows-tools.antivirus`


Ejemplo de configuracion json
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

## Funcionamiento

El challenge hace una llamada a *windows_tools.antivirus.get_installed_antivirus_software()*, que es una función de alto nivel que proporciona la lista de antivirus instalados en el equipo y los almacena en un array. Una vez hecho esto, se genera una clave que contiene el nombre de dichos antivirus y si se encuentran activos o no. 
