# Pythone
Python è un linguaggio interpretato quindi serve un interprete per analizzare ed eseguire il codice Python. Il fatto che il codice Python possa essere creato in qualsiasi editor di testo e che gli interpreti Python siano disponibili per molti sistemi operativi, consente agli sviluppatori Python di creare e distribuire programmi Python praticamente in qualsiasi sistema operativo. 
Dopo che l'interprete Python è stato installato, funziona in qualche modo come la shell di Linux. Ciò significa che quando viene chiamato senza argomenti, legge ed esegue i comandi in modo interattivo; quando chiamato con un argomento nome file o con un file come input standard, legge ed esegue uno script da quel file. Per avviare l'interprete, digita semplicemente python o python 3 al prompt della shell. 
Quando l'interprete Python viene chiamato senza argomenti e i comandi vengono immessi tramite la tastiera, si dice che l'interprete è in modalità interattiva. In questa modalità, l'interprete attende i comandi. Il prompt principale è rappresentato da tre segni di maggiore di (>>>) che indicano che l’interprete è pronto e attende i comandi. Le linee di continuazione sono rappresentate da tre punti (...). La continuazione è il prompt secondario predefinito. L'interprete riceve ed esegue istruzioni in modo interattivo.
L'interprete funge anche da semplice calcolatrice. Puoi digitare un'espressione su di essa e scriverà il valore. La sintassi delle espressioni è semplice. Gli operatori +, -, * e / funzionano esattamente come nella maggior parte degli altri linguaggi
Python non usa il ; a fine di ogni riga, si usa # per il commento sulla riga e """ per commentare più righe

VARIABILI
Le variabili vanno sempre valorizzate o genereranno un errore
#tipo: stringa
saluto = "Ringrazimo il \"collega\""  #la \ evita che il carattere venga preso come carattere speciale ma lo interpreta come semplice carattere 
print(saluto)


nome "Kirki" 
print("Il mio nome è "+nome)
#tipo: numerico
eta = 17
print("Ho "+str(eta) +" anni")
#tipo: booleano
figata = True
print("Questa cosa è una figata? "+str(figata))

per dichiarare delle variabili, anche di tipi diversi, basta scrivere il nome e in ordine il valore
"""stringa = "Bro"
   numero = 21
   booleano = true"""
stringa, numero, booleano = "Bro", 21, True

se le variabili sono uguali si può usare anche una sola dichiarazione
#primo = 20
#secondo = 20
#terzo = 20
primo = secondo = terzo = 20

TUPLES (sequenza di oggetti, anche di tipo diverso, immutabili) 
tup1 = ('prima', 'seconda', 300, 43465)
tup2 = (15, 19, 16, 655, 636)
print(tup2[1:5]) #vengono stampati gli oggetti dal 1 (compreso) al 5 (escluso) 
(output: (19, 16, 655, 636) )

LIST
figa = [1, 2, 4, 5, 6, 2, 54] #lista modificabile in future
figa[2] = 6 
print(figa[2] + " funziona")
(output: 6 funziona ) 

SETS/INSIEMI (elemento che non può comprendere più elementi uguali) 
x = [1, 2, 3, 1, 2, 3, 1, 2, 3] #questa è ancora una lsita modificabile
y = set(x) #y è un set basato su x (leva tutti i doppioni)
print(y)
(output: {1, 2, 3} )

DA CHIEDERE
x = [("Uccello", "Gatto", "Cane", "Cane", "Uccello", "Uccello")]
print(set(x))

DICTIONARY (simil json: ogni elemento ha una combinazione di valore e chiave unica)
dict = {'Eta' : 17, 'Citta' : 'Rovereto', 'Anno' : 2022}


#cambiare un elemento
dict['Anno'] = 2023


#aggiungere un elemento
dict['Sport'] = "Nuoto"
print(dict)
(output: {'Eta': 17, 'Citta': 'Rovereto', 'Anno': 2023, 'Sport': 'Nuoto'} )

INPUT
name = input("What's your name? ")
age = int(input("How old are you? "))
height = float(input("How tall are you? "))


print("Hello "+name)
print("You are "+str(age)+" years old")
print("You are "+str(height)+" cm tall")

CICLI
I cicli in python non hanno bisogno di parentesi ma vanno in base all’indentazione. (La logica è come java)
IF 
age = int(input("How old are you? "))
if age >= 18:
    print("Sei maggiorenne")
elif age < 0: #corrisponde all’else if e se ne possono usare più di uno
    print("Non sei ancora nato")
else:
    print("Non sei maggiorenne")




CICLO FOR
Il ciclo for incrementa di 1 automaticamente e ha la seguente sintassi (nel metodo range non devono esserci spazi)  
for i in range(10): #parte da 0 e arriva al numero scritto nel range (numero escluso)
    print(i) #nel ciclo
print(“Fuori”) #fuori dal ciclo


for i in range(10,20): #parte dal primo numero(incluso) e arriva al secondo (escluso)
    print(i)

for i in range(10,51,2): #parte dal primo numero(incluso) e arriva al secondo (escluso), saltando di 2 in due
    print(i)

for i in "Bro Code" : #i diventerà mano a mano le varie lettere della stringa
    print(i)

import time #import della libreria time (per usare time.sleep)
for seconds in range(10,0,-1): #python aumenta di 1 in automatico, quindi, se vogliamo aumentare o decrementare un'altro numero dobbiamo specificarlo
    print(seconds)
    time.sleep(1) #usiamo il time.sleep per fare in modo che aspetti 1 secondo prima di andare avanti
print("Happy New Year!")

WHILE
while 1 == 1: #andrà avanti all'infinito
    print("Aiuto, sono bloccata in un loop")

name = ""
while len(name) == 0: #finché il nome avrà lunghezza 0 (len() corrisponde al .length() )
    name = input("Inserisci il tuo nome: ")
print("Ciao " +name)
quello scritto sopra si può scrivere anche così:
name = None
while not name:
    name = input("Inserisci il tuo nome: ")
print("Ciao " +name)

FUNZIONI
def aggiungi_numero():
    a = 8
    b = 3
    return a+b


print (aggiungi_numero())

