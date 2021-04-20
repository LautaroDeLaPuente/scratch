# IMPORTANT
### CONFIG.JSON
```json
{
	"prefix": "!", <- TU PREFIX
	"token": "", <- EL TOKEN DE TU APP
	"devID": "" <- TU ID
}

```
### COMMAND.JS
```js
module.exports = {
	name: 'nombre del comando',
	description: 'lo que hace el comando',
	aliases: ['alias 1', 'alias 2'], <- OTROS NOMBRES POR LOS QUE EJECUTAR TU COMANDO
	guildOnly: true, <- SI SE PUEDE EJECUTAR UNICAMENTE EN SERVERS
	cooldown: 5,
	args: true, <- SI EL COMANDO ESPERA ALGÚN ARGUMENTO
	usage: '<argumento1> [argumento2]' <- EL USO QUE SE LE DEBE DAR AL COMANDO(NO PONGAS EL PREFIX, EL BOT YA LO HACE Y <> SON PARA OBLIGATORIAS Y [] PARA OPCIONALES)
	devOnly, true, <- SI SOLO LA PERSONA DEFINIDA EN `config.json` DENTRO DE `devID` PUEDE USAR EL COMANDO
	execute(message, args) { 
		// ... <- CODIGO
	},
};

```
