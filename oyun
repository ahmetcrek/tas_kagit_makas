import random
import time

tas_kagıt_makas = ["taş","kağıt","makas"]

taş = tas_kagıt_makas[0]
kağıt = tas_kagıt_makas[1]
makas = tas_kagıt_makas[2]

computer = 0
player = 0

oyuncuismi = input("Oyuncu Adınız:")

def sonuclar():
    if(computer > player):
        print ("{} - {} Bilgisayar önde.".format(computer,player))
    elif(computer == player):
        print("{} - {} durum berabere.".format(computer,player))
    elif(player > computer):
        print("{} - {} {} önde.".format(player,computer,oyuncuismi))

while True:
    devam_tamam = int(input("Oyuna devam etmek için 1'e, bitirmek için 2'ye, sonuçları görmek için 3'e basınız."))

    if(devam_tamam == 1):
        secim = input("taş-kağıt-makas?")
        a = random.choice(tas_kagıt_makas)
        print("Bilgisayar seçimini yapıyor...")
        time.sleep(2)
        print("Bilgisayar {} seçti".format(a))

        if(secim == "taş"):
            if(secim == a):
                print("Berabere :D, puan alamadınız.")
            elif(a == "kağıt"):
                print("Kağıt taşı sarar. Kaybettiniz. :((")
                computer += 1
            elif(a == "makas"):
                print("Taş makası kırar. Kazandınız. :))")
                player += 1

        elif (secim == "makas"):
            if (secim == a):
                print("Berabere :D, puan alamadınız.")
            elif (a == "taş"):
                print("Taş makası kırar. Kaybettiniz. :((")
                computer += 1
            elif (a == "kağıt"):
                print("Makas kağıtı keser. Kazandınız. :))")
                player += 1

        elif (secim == "kağıt"):
            if (secim == a):
                print("Berabere :D, puan alamadınız.")
            elif (a == "taş"):
                print("Kağıt taşı sarar. Kazandınız. :))")
                player += 1
            elif (a == "makas"):
                print("Makas kağıtı keser. Kaybettiniz. :((")
                computer += 1

        else:
            print("Geçersiz İşlem")

    elif(devam_tamam == 3):
        sonuclar()

    elif(devam_tamam == 2):
        print("""*********************************************************************
        
                              OYUN BİTTİ
        
              
                     BİLGİSAYAR: {} - {}: {}
        
        
        
*********************************************************************""".format(computer,oyuncuismi,player))
        print("İyi oyundu.")
        break
