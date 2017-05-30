# C# Style Guide

Guida di riferimento per i progetti C# (Visual Studio) in Tiknil.

### References

*  [C# Guide](https://docs.microsoft.com/en-gb/dotnet/articles/csharp/)

### Code Snippet

#### C# elements in correct order

Per semplificare l'utilizzo dell'organizzazione del codice consigliamo di utilizzare il Code Template per C# in accordo con la [StyleCop Rules Documentation](http://stylecop.soyuz5.com/SA1201.html).
La procedura per aggiungere un Code Template in Visual Studio è la seguente:

1. **Visual Studio** -> **Preferences**
2. Espandere **Text Editor**
3. Selezionare **Code Snippets**
4. Cliccare il pulsante **Add**

Si consiglia di definire il Code Template come segue:

* Shortcut: `def`
* Group: `C#`
* Mime: `text/x-csharp`
* Is expandable template: `true`
* Template Text: utilizzare il file `def.txt` contenuto in questa repo,

Per utilizzare lo snippet è necessario digitare la shortcut (es.:`def`) e premere 2 volte il tasto <kbd>Tab</kbd> per confermare e aggiungere il Template Text nel codice.

### Interface implementation
Quando si crea una classe che implementa un'interfaccia è buona norma riportare tutte le implementazioni dei metodi dell'interfaccia nella stessa area di codice. In `C#` è possibile utilizzare le `partial class` per raggiungere questo obiettivo.
Esempio:
```csharp
// Interfaccia
public interface IAawesomeInterface
{
  void AwesomeMethod();
}

// Classe partial contenente le funzionalità principali della classe
public partial class AwesomeClass
{
  // Funzionalità principali della classe
}
 
// Classe partial che implementa l'interfaccia
public partial class AwesomeClass : IAawesomeInterface
{
    public void AwesomeMethod()
    {
        // Implementazione del metodo definito nell'interfaccia
    }
}
```
