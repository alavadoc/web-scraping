# web-scraping
## Pràctica de l'assignatura de Tipologia i cicle de vida de les dades del màster de Ciència de Dades a la UOC.

Implementa un exemple de procés de web scraping que obté els valors reportats pel Consorci Sanitari de l’Alt Penedès [CSAP](http://www.csap.cat/ciutadania/temps-espera.html) a la seva web de ciutadania, referents al número de pacients existents en espera de ser visitats al seu departament d'urgències, així com els temps d'espera per a pacients adults i pediàtrics. 
Per poder executar aquest codi implementant amb el llenguatge Python serà necessari importar, i per tant, tenir les següents llibreries instal·lades a l'equip que serà executat:

```
import urllib.request as urllib2
import datetime
import csv
import time
import re
import os
from bs4 import BeautifulSoup
```
Les variables que extreu són les següents:

- Data d'actualització de la web.
- Data de la captura de dades.
- Hora de la captura de dades.
- Número de pacients en espera de Nivell 1.
- Número de pacients en espera de Nivell 2.
- Número de pacients en espera de Nivell 3.
- Número de pacients en espera de Nivell 4 i 5.
- Temps informat d'espera per a pacients adults.
- Temps informat d'espera per a pacients pediàtrics.

El programa permet escollir el període de captura de dades entre una data-hora d'inici i una data-hora de fi de procés, i permet també escollir la freqüència de captura en minuts.
