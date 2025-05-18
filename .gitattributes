#Bioloģijas tests
import random

def ievadi_vardu():
    vards = input("Ievadi savu vārdu: ")
    return vards

def biologijas_tests():
    jautajumi = [
        {
            "jautajums": "Kāds orgāns sūknē asinis cilvēka ķermenī?",
            "atbilde": "sirds"
        },
        {
            "jautajums": "Kāds ir DNS pilnais nosaukums?",
            "atbilde": "dezoksiribonukleīnskābe"
        },
        {
            "jautajums": "Kurš orgāns atbild par skābekļa apmaiņu?",
            "atbilde": "plaušas"
        },
        {
            "jautajums": "Cik kāju ir kukainim?",
            "atbilde": "6"
        }
    ]

    pareizi = 0
    for jaut in jautajumi:
        atbilde = input(jaut["jautajums"] + " ").strip().lower()
        if atbilde == jaut["atbilde"]:
            pareizi += 1

    return pareizi, len(jautajumi)

def iedrosinosha_zina(vards, pareizi, kopskaits):
    procenti = pareizi / kopskaits * 100
    if procenti == 100:
        zinas = [
            f"Teicami, {vards}! Tu esi īsts bioloģijas guru!",
            f"Perfekts rezultāts, {vards}! Tā turpini!"
        ]
    elif procenti >= 66:
        zinas = [
            f"Labi padarīts, {vards}! Tu zini daudz par bioloģiju.",
            f"Tu esi uz pareizā ceļa, {vards}!"
        ]
    else:
        zinas = [
            f"Nekas, {vards}, nākamreiz būs labāk!",
            f"Turpini mācīties, {vards}, tev izdosies!"
        ]
    print(random.choice(zinas))

def galvena():
    vards = ievadi_vardu()
    pareizi, kopskaits = biologijas_tests()
    print(f"\n{vards}, tu atbildēji pareizi uz {pareizi} no {kopskaits} jautājumiem.")
    iedrosinosha_zina(vards, pareizi, kopskaits)

if __name__ == "__main__":
    galvena()
