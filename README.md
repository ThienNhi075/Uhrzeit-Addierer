# Uhrzeit-Addierer

#Hier wird eine Funktion definiert welche zu einer Uhrzeit eine Anzahl Minuten addiert
def uhrzeit_minuten_addieren(stunden, minuten, summand):
    #Die neue Minutenanzahl könnte über 60 sein, deshalb wird das geprüft und jeweils korrigiert
    while minuten+summand >= 60:
        stunden=stunden+1
        minuten=minuten-60
        #While Schleife damit es nicht nur einmal durchgeführt wird sondern solang bis Zahl unter 60
    if stunden >= 24:
        stunden=stunden-24
        #Stunden könnten über 24 sein
    print(stunden, minuten+summand)


uhrzeit_minuten_addieren(17, 32, 8) # 17:32 + 8 Min = 17:40
uhrzeit_minuten_addieren(19, 7, 63) # 19:07 + 63 Min = 20:10
uhrzeit_minuten_addieren(16, 10, 1111) # 16:10 + 1111 Min = 10:41
