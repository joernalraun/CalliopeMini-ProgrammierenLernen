# Platzhalter / Variablen 

## Erklärung

Wenn man den Taschenrechner etwas universeller haben will, dann muss man mehr Flexibilität haben.  
D.h man muss mit verschiedenen, unterschiedlichen Werten arbeiten können.  
Anstatt den Programm-Code immer abzuändern und die Berechnung jedesmal neu zu übersetzen, brauchen wir sogenannte Platzhalter.
Platzhalter nennt man beim Programmieren auch Variablen, weil die Platzhalter unterschiedliche Werte, variable Werte aufnehmen kann.  
Das kann man sich z.B. beim einfachen Zählen mit zwei Händen vorstellen:  

- Jede Hand ist ein Platzhalter.  
- Jede Hand kann in diesem Fall Werte bis 5 "aufnehmen" (Wertebereich des Platzhalters von 0-5)
- Die beiden Hände können unterschiedliche Werte "aufnehmen"
- Nachdem beiden Händen Werte "zugewiesen" wurden, kann man mit den Platzhaltern rechnen.
- Linke_Hand + Rechte_Hand = Gesuchte Summe
- In der Programmierung wird das ganze dann umgedreht :
- Gesuchte Summe = Linke_Hand + Rechte_Hand  

## Die Hände

![Linke Hand](pics/ZaehlendeHaende_L.png)

![Rechte Hand](pics/ZaehlendeHaende_R.png)

## Zuweisung

Damit Platzhalter Werte aufnehme können, werden ihnen Werte zugewiesen.  
Das geschieht in der Programmierung mit dem Gleichheitszeichen.
Dieses Gleichheitszeichen ist nicht zu verwechseln mit dem Gleichheitszeichen in der Mathematik.  
Das Gleichheits-Zeichen beim Programmieren bedeutet, dass dem Platzhalter auf der linken Seite der Wert auf der rechten Seite des Gleichheits-Zeichens zu gewiesen wird.

Beispiel 1: 

Linke Hand = 3  

![Linke Hand](pics/LinkeHand_3.png)

heisst : Ab jetzt hat der Platzhalter Linke Hand den Wert 3.

Beispiel 2:

Rechte Hand = 5 

![Rechte Hand](pics/RechteHand_5.png)

heisst : Ab jetzt hat der Platzhalter Rechte Hand den Wert 5.

## Addition mit Platzhaltern 

Anstatt 3 + 5 heisst unsere Rechnung nun:

Linke Hand + Rechte Hand = Gesuchte Summe

Um daraus einen Programmiervorschrift zu machen, dreht man die beiden Teile um das Gleichheits-Zeichen herum, also:

Gesuchte Summe = Linke Hand + Rechte Hand 

Diese eine Berechnungs-Anweisung / Formel ist unser "Programm" und ist für völlg verschiedene Werte von Rechte Hand und Linke Hand durchführbar.
Man kann die Zuweisungen irgendwann beim Programm-Start machen und erst viel später (wenn man als Mensch schon lange die Werte vergessen hat) die beide Platzhalter addieren.


## Auswahl aus Menu

![Menu-Anlegen](pics/PlatzhalterAnlegenMenu.png)

![Menu-Benennen](pics/PlatzhalterBenennenMenu.png)

![Menu-Benennen](pics/PlatzhalterBenennenMenu_2.png)

![Menu-Zuweisung](pics/PlatzhalterZuweisungMenu.png)

![Menu-ZuweisungAuswahl](pics/PlatzhalterVerwendenZuweisungMenu.png)

## Verwendung des Platzhalters 

![Menu-Verwenden](pics/PlatzhalterBenutzenMenu.png)

Verwendung der Variablen Ausgaben und Berechnungen anstatt fester Werte.


![Menu-Verwenden-2](pics/PlatzhalterBenutzenMenu_2.png)

Dazu zieht man die Variable/den Platzhalter genau an die Stelle an der vorher feste Werte benutzt wurden.



## PXT-Code

Finales simples Taschenrechner-Programm.  
Immernoch muss Programm-Code geändert werden um eine neue Berechnung durchzuführen, aber die Werte für die Berechnung müssen nur an einer zentralen Stelle geändert werden.
Dank Verwendung von Platzhaltern/Variablen passt sich die Ausgabe jeweils entsprechend an.



![Zwischenfinales Programm mit Platzhalter](pics/Platzhalter_Final.png)



## JavaScript-Code

<details>
 <summary>Java-Script-Code</summary>

```js
let rechteHand = 0
let linkeHand = 0
basic.forever(() => {
    linkeHand = 3
    rechteHand = 4
    basic.showNumber(linkeHand)
    basic.showString(" + ")
    basic.showNumber(rechteHand)
    basic.showString(" = ")
    basic.showNumber(linkeHand + rechteHand)
    basic.clearScreen()
    basic.pause(1000)
})
```
</details>

## Download Hex-Code

![Hex-code](mini-PlatzhalterFinal.hex)



