# Fondamenti di Informatica T-1 · C

[English](README.md) · **Italiano**

Una piccola libreria C e uno "startkit" per l'esame, scritti per *Fondamenti di Informatica T-1* all'Università di Bologna (Ingegneria Informatica, 2022–23). È stato il mio primo contatto con la programmazione e con GitHub. Fa parte del mio [materiale universitario](https://github.com/CometaSensitiva/university).

## Contenuto

| Cartella | Contenuto |
| --- | --- |
| [`Libreria/`](Libreria) | Tipo di elemento generico con compare/assign/swap, array dinamici, algoritmi di ordinamento (naive, bubble, insertion, merge, quick sort) e ADT lista |
| [`Esame/`](Esame) | La libreria applicata al testo di un esame passato: lettura da file, gestione di liste e struttura tipica di una soluzione |

La libreria è costruita attorno a un tipo di elemento sostituibile (`myType`, `mySecondType`): le stesse funzioni di ordinamento e di lista si adattano ai record di ogni testo d'esame.

## Come usarlo

Lo startkit si adatta a quasi tutti gli esami degli anni passati: bastano un paio di prove pratiche per prendere la mano.

<details>
<summary>Configurazione in Visual Studio, passo per passo</summary>

1. Scarica questa repository sul tuo computer.
2. Crea un nuovo "Progetto vuoto" in Visual Studio e spunta "Inserisci soluzione e progetto nella stessa directory".
3. In "Esplora soluzioni" seleziona ed elimina le cartelle "Dipendenze esterne", "File di intestazione", "File di origine" e "File di risorse".
4. Tasto destro sul nome del progetto → Aggiungi → Nuovo filtro, e crea il filtro "Libreria". Ripeti per creare il filtro "Esame".
5. Tasto destro sul nome del progetto → Apri cartella in Esplora file, e copia lì tutti i singoli file `.c` e `.h` di `Esame` e `Libreria` (i file, non le cartelle).
6. Tasto destro sul filtro "Esame" → Aggiungi → Elemento esistente, e seleziona i file di `Esame` (`element.c`, `element.h`, `file1.txt`, `file2.txt`, `funzioni.c`, `funzioni.h`, `lib.c`, `lib.h`, `list.c`, `list.h`, `main.c`).
7. Ripeti con il filtro "Libreria" e i file di `Libreria` (`aMyLib`, `bMyType`, `cMySecondType`, `dMyList`, `.c` e `.h`).
8. Sei pronto per l'esame. Buona fortuna!

</details>
