# C# Style Guide

Guida di riferimento per i progetti C# (Xamarin Studio) in Tiknil.

### References

*  [C# Guide](https://docs.microsoft.com/en-gb/dotnet/articles/csharp/)

### Code Snippet

#### C# elements in correct order

Per semplificare l'utilizzo dell'organizzazione del codice consigliamo di utilizzare il Code Template per C# in accordo con la [StyleCop Rules Documentation](http://stylecop.soyuz5.com/SA1201.html).
La procedura per aggiungere un Code Template in Xamarin Studio è la seguente:

1. **Xamarine Studio** -> **Preferences**
2. Espandere **Text Editor**
3. Selezionare **Code Templates**
4. Cliccare il pulsante **Add**

Si consiglia di definire il Code Template come segue:

* Shortcut: `def`
* Group: `C#`
* Mime: `text/x-csharp`
* Is expandable template: `true`
* Template Text: utilizzare il file `code-templete.txt` contenuto in questa repo,

Per apportare le modifiche è necessario riavviare Xamarin Studio.

Per utilizzare lo snippet è necessario digitare la shortcut (es.:`def`) e premere 2 volte il tasto <kbd>Tab</kbd> per confermare e aggiungere il Template Text nel codice.
