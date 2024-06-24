## Hashverfahren
MD2, SHA-1, SHA-256 (Beispielverfahren)

## Ergebnis
### MD2
Eingabetext: `Wir sind im TBZ Modul`

- Hashwert der Originaldatei: `A4 AD BB E4 3E 6D CA E5 75 40 CE 7B C2 51 E7 31`
- Hashwert der Aktuellen Datei: `84 89 C7 CA 12 31 D2 69 17 BB 6C 27 D8 1B 30 A4 `


### SHA-1
- Hashwert der Originaldatei: `32 E3 A0 10 A0 D3 4B 99 99 C7 06 F4 DE AA A8 18 D4 6C 36 B1`
- Hashwert der Aktuellen Datei: `C2 DF C7 36 8A FF 00 3B 07 B3 A1 E7 4F 12 AD A7 67 D3 09 E9`

### SHA-256
- Hashwert der Originaldatei: `D9 4D 8D B6 52 C0 14 E1 DD 87 D9 31 6B B4 55 AB C3 7B 81 60 BD AB 48 AB 98 16 4D 8D 45 84 AB 96`
- Hashwert der Aktuellen Datei: `E6 E1 C6 E7 FB CD CC CA 45 AE A0 42 89 31 0C 99 A0 0B 10 F6 00 69 BF 0A D8 75 BC 74 0A 3F BE 9D`


## Interpretation
- **MD2**: MD2 ist ein älterer Algorithmus, der ursprünglich für Systeme mit wenig Speicher entwickelt wurde. Trotz seiner Einfachheit gilt MD2 heute als veraltet und unsicher, insbesondere gegen moderne Angriffe. Er wird kaum noch in sicherheitskritischen Anwendungen eingesetzt.

- **SHA-1**: SHA-1 wurde als Nachfolger von MD5 entwickelt und bot eine Zeit lang mehr Sicherheit. Allerdings wurde auch SHA-1 als anfällig gegen Angriffe eingestuft und wird daher nicht mehr für sicherheitsrelevante Anwendungen empfohlen. Einige ältere Systeme verwenden SHA-1 noch, aber es wird dringend empfohlen, auf sicherere Alternativen umzusteigen.

- **SHA-256**: SHA-256 ist ein Teil der SHA-2-Familie und gilt derzeit als einer der sichersten Hash-Algorithmen. Er bietet einen hohen Sicherheitsstandard und wird in vielen sicherheitskritischen Anwendungen, wie SSL/TLS-Zertifikaten und Kryptowährungen, weit verbreitet eingesetzt. SHA-256 wird als moderner und sicherer Algorithmus angesehen und ist die empfohlene Wahl für neue Anwendungen.
