# Projekt PWI: Bridge Teacher


## Cel projektu

Napisz program wspomagający naukę licytacji brydżowej, zgodnej ze standardem [Wspólny Język (WJ)](https://jassem.pl/wp-content/uploads/2019/12/wj2020-25-59.pdf).


Program na wejsciu otrzymuje:

- plik w formacie [pbn](#pbn),
- (opcjonalnie) wartość zmiennej **Dealer** (od którego gracza zaczyna się licytacja),
- pozycję gracza.

Program pokazuje graczowi:

- jego karty,
- licytację przeciwników

i oczekuje na odzywkę gracza, a następnie pokazuje czy wskazana odzywka jest zgodna ze standardem WJ.


Zaprojektuj program tak, aby można było łatwo wprowadzać zmiany do strategii licytowania.



## Dodatkowe informacje

### Format PBN (#pbn)

Pliki w formacie **Portable Bridge Notation** [pbn_v21](https://www.tistis.nl/pbn/)
są plikami tekstowymi, które przechowują informacje dotyczące brydżowego rozdania. Przykładowy [plik](bridge/pbn7198348092905869869.pbn):

```pbn
% PBN 2.1
% Created by: NeuralPlay Bridge
% https://www.neuralplay.com 
[Event "Unknown"]
[Site "Unknown"]
[Date "2022.12.10"]
[Board "1"]
[West "Unknown"]
[North "Unknown"]
[East "Unknown"]
[South "Unknown"]
[Dealer "N"]
[Vulnerable "None"]
[Deal "N:AJ965.A4.KQT3.K2 K4.97653.52.J984 Q8.K8.A98764.A63 T732.QJT2.J.QT75"]
[Scoring "MP"]
[Declarer "S"]
[Contract "6D"]
[Result "12"]
{
Board: 1            S: AJ965
Dealer: N           H: A4
Vul: None           D: KQT3
                    C: K2


S: T732                                 S: K4
H: QJT2                                 H: 97653
D: J                                    D: 52
C: QT75                                 C: J984


                    S: Q8
                    H: K8
                    D: A98764
                    C: A63
}
[Auction "N"]
1C =1=    Pass      2D =2=    Pass
2S =3=    Pass      4D =4=    Pass
5D =5=    Pass      6D =6=    Pass
Pass      Pass      
[Note "1:Shows 17+ hcp or 16+ hcp with a 5+ card suit."]
[Note "2:Shows 8+ hcp and 5+ cards in the suit."]
[Note "3:Shows 5+ cards in the suit and 17-19 points."]
[Note "4:Shows 6+ cards in the suit and 11+ points."]
[Note "5:Minor game. Shows 28+ points combined with partner."]
[Note "6:Small slam. Shows an 8+ card fit in the suit and 33+ points combined with partner."]
[Play "W"]
HQ H4 H3 HK
DJ DK D2 D4
S2 D3 D5 D6
S3 S5 SK SQ
CQ CK C4 C3
C5 C2 C8 CA
C7 DT C9 C6
H2 HA H5 H8
S7 SA S4 S8
ST S6 H6 D7
CT DQ H7 D8
HT S9 H9 D9
HJ SJ CJ DA
*
```

Powyższy plik zawiera zarówno informacje o rozdanych kartach jak i przebiegu licytacji (zgodnie z innym schematem licytowania), oraz przebiegu samego rozdania.
