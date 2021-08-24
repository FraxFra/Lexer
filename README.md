# Lexer
Il lexer o analizzatore lessicale analizza sequenze di caratteri e stampa in output token.
In particolare controlla la correttezza grammaticale di costrutti sintattici andando a generare un errore dove il lessema non è riconosciuto dall'automa.
L'automa è una frazione di codice che controlla autonomamente la correttezza delle parole e in questo caso è implementato nel Lexer.
Per poter eseguire il programma seguire i seguenti passaggi:
        - Scaricare tutti i file nella propria directory principale
        - Compilare tutti i file da terminale attraverso il comando "javac NomeFile.java" lasciando Lexer.java per ultimo
        - Scrivere del codice generico in un linguaggio di programmazione a scelta e salvarlo all'interno del file Prova.txt
        - Eseguire Lexer.java attraverso il comando "java Lexer" grazie al quale si otterrà la sequenza di token
A questo punto, attraverso l'osservazione dei token, sarà possibile trarre due conclusioni:
        - Il Lexer è arrivato a fine file (ultimo token stampato: "<-1>") e tutte le parole inserite all'interno del file di prova sono state riconosciute
        - Il Lexer non è arrivato a fine file (si è generato un errore) e una determinata parola inserita all'interno del file di prova non è stata riconosciuta
