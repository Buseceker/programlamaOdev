# programlamaOdev
import random

def deste_tanimla():
    sayilar = ("1","2","3","4","5","6","7","8","9","10","vale","kiz","papaz")
    simgeler = ("maca","karo","kupa","sinek")
    kartlar = []
    for i in range(4):
        for j in range(13):
            kartadi = simgeler[i] + " " + sayilar[j]
            kartlar.append(kartadi)
    return kartlar


def kart_karistir(deste):
    random.shuffle(deste)
    return

def kart_cek(deste):
    return deste.pop(0)

deste=deste_tanimla()
kart_karistir(deste)

for i in range(4):
    print str(i+1) + ".oyuncu"
    for j in range(13):            
        kart = kart_cek(deste)
        print kart
    print ""
