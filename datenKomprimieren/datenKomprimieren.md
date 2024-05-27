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

## 4. RLC
Weiß: 0, Schwarz: 1
0 0 0 0 0 0 0 0
1 1 1 1 1 1 1 0
0 0 0 0 0 0 0 0
1 1 1 1 1 1 1 1
0 0 0 0 1 1 1 1
1 1 1 1 1 1 1 1
0 0 0 0 0 0 0 0
1 1 1 1 1 1 1 0

⬜⬜⬜⬜⬜⬛⬛⬜  
⬛⬛⬛⬛⬛⬛⬛⬜  
⬛⬜⬜⬜⬜⬛⬛⬜  
⬜⬜⬜⬜⬛⬜⬜⬜  
⬜⬜⬜⬜⬛⬜⬜⬜  
⬜⬜⬜⬜⬛⬜⬜⬜  
⬜⬜⬜⬜⬛⬜⬜⬜  
⬜⬜⬜⬜⬛⬜⬛⬛

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
