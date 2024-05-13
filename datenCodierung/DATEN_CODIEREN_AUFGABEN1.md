# Daten Codieren NUM

## 1

| Dezimal | Hex   | Binär  | Binär  | Binär  | Binär  |
|---------|-------|--------|--------|--------|--------|
| 0       | 0     | 0      | 0      | 0      | 0      |
| 1       | 1     | 1      | 1      | 1      | 1      |
| 2       | 2     | 10     | 10     | 10     | 10     |
| 3       | 3     | 11     | 11     | 11     | 11     |
| 4       | 4     | 100    | 100    | 100    | 100    |
| 5       | 5     | 101    | 101    | 101    | 101    |
| 6       | 6     | 110    | 110    | 110    | 110    |
| 7       | 7     | 111    | 111    | 111    | 111    |
| 8       | 8     | 1000   | 1000   | 1000   | 1000   |
| 9       | 9     | 1001   | 1001   | 1001   | 1001   |
| 10      | A     | 1010   | 1010   | 1010   | 1010   |
| 11      | B     | 1011   | 1011   | 1011   | 1011   |
| 12      | C     | 1100   | 1100   | 1100   | 1100   |
| 13      | D     | 1101   | 1101   | 1101   | 1101   |
| 14      | E     | 1110   | 1110   | 1110   | 1110   |
| 15      | F     | 1111   | 1111   | 1111   | 1111   |

Alle drei Kolonnen mit Binär sind gleich

## 2

Dezimal: 911 => Binär:  11 1000 1111

## 3

Binär: 1011 0110 => Dezimal: 182

## 4

Binär: 1110 0010 1010 0101 => Hexadezimal: E2A5

## 5

Binär: 1101 1001 + 0111 0101 = 1100 1110

(Das 9. Bit wird einfach gelöscht, da nur 8 Bit zur verfügung stehen.)

## 6
a. Binär: 1100 0000 . 1010 1000 . 0100 1100 . 1101 0011 => Dezimal: **192.168.76.211** = IPv4-Adresse
b. Binär: 1011 1110 - 1000 0011- 1000 0101 - 1101 0101 1110 0100 - 1111 1110 => Hex:**BE-83-85-D5E4-FE** = MAC-Adresse

## 8

107 Gondeln => 110 1011 => Codebreite = 7

## 11

a. 0/255
b. -127/127
c. 0101 0011
d. 1101 0011
e. 1101 0011 + 0101 0011 = 1000 0000
f. 0000 0000 (Nein)
g. Weil man dafür die 8 Bits brauche, welches aber das Vorzeichen ist

## 12

Ich würde die Zahl 0.3333333 als 3333333 speichern, mit E - 7.

# Daten Codieren Alphanumerisch
### a)

- Textsample1 = ANSI
- Textsample2 = UTF8
- Textsample3 = UTF16 BE BOM

### b)

68

### c)

- Textsample1 -> ANSI => 68 bytes = 1 Byte pro Zeichen

- Textsample2 -> UTF8 => 71 bytes 1 Byte pro ASCII-Zeichen + mehr als 1 Byte pro nicht ASCII-Zeichen

- Textsample3 -> UTF16 BE BOM => 138 bytes = 2 Bytes für die meisten Zeichen + 2 Bytes am Anfang für BOM

### d)

ä, €

### e)

BE (Big-Endian) = Das höchstwertigste Byte wird zuerst gespeichert oder übertragen.

LE (Little-Endian) = Das niederwertigste Byte wird zuerst gespeichert oder übertragen.

### f)

Wenn die Datei ausschliesslich ASCII-Zeichen enthält, bleibt sie unverändert, da diese Zeichen in UTF-8 identisch sind.

Falls die Datei jedoch Zeichen enthält, die nicht im ASCII-Zeichensatz enthalten sind, aber in UTF-8 vorkommen, werden diese Zeichen nur korrekt dargestellt, wenn sie in UTF-8 codiert sind.
