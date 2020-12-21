# mysticalreader

## Memorizzazione di messaggi e traduzioni personalizzati

Come sviluppatore puoi creare un file `messages.json` che contiene il tuo testo e le tue traduzioni. Ci sono due tipi di oggetti all'interno di questo file: `DM` e` embeds`. I messaggi diretti saranno un singolo messaggio in diverse lingue, mentre gli incorporamenti conterranno diversi tipi di campi. Un esempio di ciascuno:

DM:

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
