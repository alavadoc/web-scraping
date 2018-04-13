# web-scraping
## Pràctica de l'assignatura de Tipologia i cicle de vida de les dades del màster de Ciència de Dades a la UOC.

Implementa un exemple de procés de web scraping que obté els valors reportats pel Consorci Sanitari de l’Alt Penedès [CSAP](http://www.csap.cat/ciutadania/temps-espera.html) , referents al número de pacients existents en espera de ser visitats al seu departament d'urgències, així com els temps d'espera per a pacients adults i pediàtics. 
Per poder executar aquest codi implementant amb el llenguatge Python serà necessari importar, i per tant, tenir les següents llibreries instal·lades a l'equip que serà executat:

'''
import urllib.request as urllib2
import datetime
import csv
import time
import re
import os
from bs4 import BeautifulSoup
'''
