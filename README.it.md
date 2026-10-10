# Fondamenti di Informatica T-1 · C

[English](README.md) · **Italiano**

Una piccola libreria C e uno "startkit" per l'esame, scritti per *Fondamenti di Informatica T-1* all'Università di Bologna (Ingegneria Informatica, 2022–23). È stato il mio primo contatto con la programmazione e con GitHub. Fa parte del mio [materiale universitario](https://github.com/CometaSensitiva/university).

## Contenuto

| Cartella | Contenuto |
| --- | --- |
| [`Libreria/`](Libreria) | Tipo di elemento generico con compare/assign/swap, array dinamici, algoritmi di ordinamento (naive, bubble, insertion, merge, quick sort) e ADT lista |
| [`Esame/`](Esame) | Un modello vuoto per l’esame, con sorgenti, dati d’esempio e spazi per quattro esercizi |

La libreria è costruita attorno a un tipo di elemento sostituibile (`myType`, `mySecondType`): le stesse funzioni di ordinamento e di lista si adattano ai record di ogni testo d'esame.

## Come usarlo

Per il modello d’esame, crea un progetto C vuoto in Visual Studio e aggiungi i file `.c` e `.h` di **Esame soltanto**. Tieni `file1.txt` e `file2.txt` nella cartella di lavoro del programma. `main.c` contiene spazi da completare, non una soluzione d’esame.

Con Clang o GCC, dalla cartella principale del repository:

```sh
cc -std=c11 Esame/*.c -o /tmp/esame
(cd Esame && /tmp/esame)
```

`Libreria` è una raccolta separata da adattare all’esercizio. Non unire le due cartelle in un eseguibile: contengono definizioni sovrapposte di funzioni di utilità. La libreria storica richiede inoltre la configurazione di header e tipi; la sua dichiarazione di `srand48` è in conflitto con quella di sistema su macOS e Linux.
