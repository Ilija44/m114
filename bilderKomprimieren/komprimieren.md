## Aufgaben

### 1. 

- RGB 255/255/255 entspricht Weiss und ergibt in YCbCr: **1-0-0**
- RGB 0/0/0 entspricht Schwarz und ergibt in YCbCr: **0-0-0**
- Y:0, Cb:0.5, Cr:0 entspricht der Farbe: **Rot**
- Y:0, Cb:-0.5, Cr:0 entspricht der Farbe: **Grün**
- Y:0, Cb:0, Cr:0.5 entspricht der Farbe: **Blau**
- Y:0, Cb:0, Cr:-0.5 entspricht der Farbe: **Ebenfalls Grün**
- Y:0.3, Cb:0.5, Cr:-0.17 entspricht der Farbe: **Ebenfalls Rot**

### 2.

- Rot: 33 x 0.3 = 9.9 
- Grün: 121 x 0.6 = 72.6 
- Blau: 239 x 0.1 = 23.9 
- Summe=106.4 

Somit **Graustufenwert=106**

### 3.

- Subsampling 4:1:1 bedeutet: 100% + 25% + 25% = 150% gegenüber dem Original von 3x 100%. Somit **1/2 Speicherbedarf**

### 4. 

Schauen sie den an und beantworten sie anschliessend diese Fragen:

**a. **

Nein, denn es sind immer noch drei Kanäle mit z.B. 8 Bit Auflösung pro Kanal.

**b.**

Nein! Der Beamer verwendet drei Farbkanäle/Farbkanonen im additiven Farbsystem. Darum wird RGB benötigt.

**c.**

Die Farbe Grün hat 60% Anteil am Graustufenbild, Rot 30% und Blau 10%

**d.**

Das menschliche Auge ist für Grün am meisten empfindlich. Das hat einen evolutionsbiologischen Hintergrund. Danach folgt Rot und für Blau ist man am wenigsten empfindlich, mal von den Schlümpfen abgesehen ;-)

### 5.

Schauen sie den an und beantworten sie anschliessend diese Fragen:

**a. **

Der Luminanzkanal (Graustufenkanal) hat bei beiden Varianten eine unverändert hohe Auflösung. Dies ist entscheidend für die Bildschärfe.

**b.**

Original: 100% + 100% + 100% = 300%  
Dem gegenüber 4:1:1 bedeutet 100% + 25% + 25% = 150%  
Somit belegt 4:1:1 die Hälfte des Speicherplatzes (150%) vom Original (300%)

### 6. 

Schauen sie den an und beantworten sie anschliessend diese Fragen:

**a.**

Umwandlung von RGB in YCbCr, danach Subsampling.

**b.**

Nein, es sind pro Block immer noch 8*8=64 Werte. Erst die anschliessende Quantisierung und der darauf einsetzende RLC bringt eine Datenreduktion.

**c.**

Wegen der Unterteilung in 8*8-Pixel Blöcke, die sich – vereinfacht ausgedrückt – in der Farbe immer mehr angleichen und als Quadrate im Bild wahrgenommen werden.

### 7. 

Schauen sie den an und beantworten sie anschliessend diese Fragen:

**a.**

Intraframe: Komprimierung innerhalb eines Bildes.  
Interframe: Komprimierung über eine Bildserie.

**b.**
   i. 30 Sekunden-Szene mit Faultier auf Nahrungssuche?

Hat viel Potential bei der Interframekomprimierung, weil die Bilder sich kaum unterscheiden.

   ii. 30 Sekunden-Szene mit Zieleinfahrt beim Formel-1-Rennen?

Hat wenig Potenzial, weil sich die Bilder sehr unterscheiden.

**c.**

Ja, auch beim Datenbackup muss immer mal wieder ein Fullbackup (vgl. I-Frame) erstellt werden.

**e.**

Jedes 25. Bild ist ein komplettes Bild. (I-Frame oder Schlüsselbild)
