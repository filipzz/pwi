# Projekt PWI: Bridge 


## Cel projektu

Napisz program umożliwiający przeprowadzenie rozgrywki brydżowej (bez licytacji).

Program na wejsciu otrzymuje:

- plik w formacie [pbn](#pbn),
- wylicytowany kontrakt.

Program ma co najmniej następujące tryby działania:

- umożliwia rozegranie rozdania -- użytkownik podaje zrzucane karty (program pilnuje poprawności i kolejności zagrań),
- wspiera tryb "AI" -- zaimplementuj algorytm, który wykonuje poprawne zagrania za wskazanych graczy (ale tak, aby
AI umiało rozegrać oczywiste sytuacje typu np. "wykładane" 7NT).
- (gdy zadziała tryb AI): program sprawdza, czy dla danego wistu AI ugra kontrakt.



## Dodatkowe informacje

### Format PBN (#pbn)

Pliki w formacie **Portable Bridge Notation** [pbn_v21](https://www.tistis.nl/pbn/)
są plikami tekstowymi, które przechowują informacje dotyczące brydżowego rozdania. Przykładowy [plik](pbn3286580313622489622.pbn):

```pbn
% PBN 2.1
% Created by: NeuralPlay Bridge
% https://www.neuralplay.com 
[Event "Unknown"]
[Site "Unknown"]
[Date "2022.12.16"]
[Board "5"]
[West "Unknown"]
[North "Unknown"]
[East "Unknown"]
[South "Unknown"]
[Dealer "N"]
[Vulnerable "NS"]
[Deal "N:J9.A8.A97542.AJ8 654.9652.KQJ8.53 AKQ7.KQ74..KQ762 T832.JT3.T63.T94"]
[Scoring "MP"]
[Declarer "S"]
[Contract "7NT"]
[Result "13"]
{
Board: 5            S: J9
Dealer: N           H: A8
Vul: NS             D: A97542
                    C: AJ8


S: T832                                 S: 654
H: JT3                                  H: 9652
D: T63                                  D: KQJ8
C: T94                                  C: 53


                    S: AKQ7
                    H: KQ74
                    D: 
                    C: KQ762
}
[Auction "N"]
1D =1=    Pass      3C =2=    Pass
4D =3=    Pass      4NT =4=   Pass
6C =5=    Pass      7NT =6=   Pass
Pass      Pass      
[Note "1:Shows 11-15 hcp. Could be short (as few as one diamond in rare cases)."]
[Note "2:Shows 16+ hcp and 5+ cards in the suit. Game forcing."]
[Note "3:Shows 6+ diamonds and 14+ points."]
[Note "4:Shows 25+ points combined with partner."]
[Note "5:Small slam. Shows an 8+ card fit in the suit and 33+ points combined with partner."]
[Note "6:Grand slam. Shows 37+ points combined with partner."]
[Play "W"]
S2 SJ S4 S7
H3 HA H2 H4
C4 CJ C3 C2
C9 CA C5 C6
D3 DA D8 H7
CT C8 S5 CK
D6 H8 S6 CQ
DT S9 H5 C7
HT D2 H6 HQ
HJ D4 H9 HK
S3 D5 DJ SQ
S8 D7 DQ SK
ST D9 DK SA
*
```

Powyższy plik zawiera zarówno informacje o rozdanych kartach jak i przebiegu licytacji (zgodnie z innym schematem licytowania), oraz przebiegu samego rozdania.
