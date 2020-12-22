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

Puoi trovare il default `messages.json` qui: https://github.com/simoyoshi/mysticalreader/blob/main/messages.json. Puoi cambiare il tuo `messages.json` così:

```JS
new MysticalReader(client, 'commands', 'features', 'messages.json')
```
