# Daten Komprimieren 

## 1. Huffman-Algorithmus

Dateisysteme haben auch eine Baumstruktur.

Ein binärer Baum hat bei jedem Knoten, immer höchstens 2 Kinder, dies ist bei nicht binären Bäumen nicht so, da gibt es meistens keine Begrenzung von Kindern.

## 2. Huffman-Algorithmus

### Encode Huffman-Algorithmus
![image](https://github.com/Ilija44/m114/assets/113606362/9f7ffb68-5506-41c4-b6aa-e77e8d952d67)

## 3. RLC
Mit 5 Bit kann man eine Linie von Pixeln im Bild darstellen. Es könnte 1 Bit oder kein Bit sein, da man einfach die Farbe angeben kann.

10100Gelb 1011Gelb, 10Schwarz, 111Gelb

10100Blau 1011Blau, 1Rot, 1Schwarz, 111Blau 100Blau, 10Rot, 1Schwarz, 10Blau, 101Rot, 1Schwarz,5Blau

1Blau

## 4. RLC:
Sie erhalten diesen RL-Code: 010100011110010010010010010010010010010110010110010010010010010010010010001 

```
010 100 011 110 010 010 010 010 010 010 010 010 010 110 010 110 010 010 010 010 010 010 010 010 001
 |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |
 2   4   3   6   2   2   2   2   2   2   2   2   2   6   2   6   2   2   2   2   2   2   2   2   1
 |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |
 W   S   W   S   W   S   W   S   W   S   W   S   W   S   W   S   W   S   W   S   W   S   W   S   W

WWSSSSWW
WSSSSSSW
WSSWWSSW
WSSWWSSW
WSSSSSSW
WSSSSSSW
WSSWWSSW
WSSWWSSW


  XXXX
 XXXXXX
 XX  XX
 XX  XX
 XXXXXX
 XXXXXX
 XX  XX
 XX  XX
```

Es wird ein 'A' dargestellt.

## 5. LZW-Verfahren

### a. 

| Zeichenkette | Gefunden | Gespeichert | Eintrag | Nummer |
| ------------ | -------- | ----------- | ------- | ------ |
| ananas       | a        | a           | an      | 256    |
| nanas        | n        | n           | na      | 257    |
| anas         | a        | 256         | ana     | 258    |
| as           | a        | a           | as      | -      |

ANANAS = an256as

### b. 

| Zeichenkette  | Gefunden | Ausgabe | Eintrag | Nummer |
| ------------- | -------- | ------- | ------- | ------ |
| erdbe256kl260 | e        | e       | -       | -      |
| rdbe256kl260  | r        | r       | er      | 256    |
| dbe256kl260   | d        | d       | rd      | 257    |
| be256kl260    | b        | b       | db      | 258    |
| e256kl260     | e        | e       | be      | 259    |
| 256kl260      | e        | er      | ee      | 260    |
| kl260         | k        | k       | ek      | 261    |
| l260          | l        | l       | kl      | 262    |
| 260           | e        | ee      | le      | 263    |

erdbe256kl260 = erdbeerdklee


# 8.
## Andere Verfahren
 - Lempel-Ziv-Welch (LZW)
 - Deflate
 - Arithmetic Coding

### Daten, die verlustlos komprimiert werden sollten
- Textdateien
- Datenbanken
- Java Source Code

### Auswirkungen verlustbehafteter Komprimierung auf Texte und Quellcode
- Wörter verlust
- Daten verlust
- Unlesbarkeit
- Unausführbarkeit von Code
- Syntaxfehler
