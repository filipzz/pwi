# PWI - Reguła d'Hondta

## Cel projektu

Napisz program, który dla wyników wyborów i parametrów systemu obliczy liczę mandatów 
dla każdego ugrupowania. 

## Działanie

Parametry systemu:

- próg wyborczy (w Polsce \(5\%,  8\%\)),
- postęp dzielnika (w Polsce arytmetyczny \(a_1 = 1, a_{i+1} = a_i + 1\); w Czechach \(a_1 = 1.42, a_2 = 2, a_3 = 3, \ldots \), ale może też być \(a_i = 2^s\))

Program ma działać zarówno dla danych wprowadzanych interaktywnie
jak i z plików (np. w formacie csv). Zaprojektuj program tak, aby można było
łatwo wskazywać dane w plikach o nieco innym formacie.

- [wyniki 2019](https://sejmsenat2019.pkw.gov.pl/sejmsenat2019/pl/dane_w_arkuszach)
- [wyniki 2015](https://parlament2015.pkw.gov.pl/355_Wyniki_Sejm_XLS.html)

