# mysticalreader

## Storing custom messages and translations

As the developer you can create a `messages.json` file that contains your own text and translations. There are two types of objects within this file: `direct messages` and `embeds`. Direct messages will be a single message in different languages, while embeds will contain different types of fields. An example of each:

Direct messages:

```JSON
{
  "NEW_LANGUAGE": {
    "english": "Language set to {LANGUAGE}.",
    "spanish": "Idioma configurado en {LANGUAGE}."
  }
}
```

Embed:

```JSON
{
  "HELP_MENU": {
    "TITLE": {
      "english": "Help Menu",
      "spanish": "Menú de ayuda"
    }
  }
}
```

You can find the default `messages.json` here: https://github.com/AlexzanderFlores/WOKCommands/blob/main/messages.json. You will also need to define where your `messages.json` file lives in the WOKCommands constructor like so:

```JS
// Assumes messages.json is in the same directory as this code's file
new WOKCommands(client, 'commands', 'features', 'messages.json')
```
