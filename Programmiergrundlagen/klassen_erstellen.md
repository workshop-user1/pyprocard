## Klassen erstellen mit *class*

Um selbst Objekte in Python (und auch anderen objektorientierten Programmiersprachen) zu erstellen, ist eine *Klasse* zu definieren. Diese erfüllt die Funktion eines *Bauplans*, aus dem konkrete Objekte erstellt werden können - die *Instanzen*.

Um mit Klassen in der Processing-IDE bequem arbeiten zu können, wird folgendes Vorgehen empfohlen:

### Klassen definieren

Zunächst erstellen wir in der Processing-IDE (Python-Mode) das Grundgerüst eines Processing-Sketches.

```python
def setup():
    pass
    
    
def draw():
    pass
```

Den Sketch speichern wir unter dem Namen `Stimmungen` ab.

Die Processing-IDE unterstützt die Verwaltung von Programmteilen wie Klassen oder Modulen durch Tabs am Kopf des Editorbereichs. Für das Smiley-Beispiel erstellen wir also einen neuen Tab und vergeben den Namen `Smiley`. Processing macht daraus den Dateinamen `Smiley.py`.

![Erstellen eines neuen Tabs in Processing](../images/neuer-tab.png)

Im Dateisystem unseres Rechners wird das Projekt nun wie folgt abgebildet:

![Aufbau des Sketches im Dateisystem](../images/oop-tree.png)

`Stimmungen.pyde` ist die Hauptdatei des Sketches, `Smiley.py` die Datei für unsere Klasse. Jetzt können wir beginnen, die ersten Zeilen für die Klasse `Smiley` zu schreiben.

```python
class Smiley:
    pass
```

Mit dem Schlüsselwort `class` gefolgt von einem bezeichnenden Substantiv beginnt die Definition. `pass` ist an dieser Stelle wieder nur ein Platzhalter für Code, der später folgt.

Unsere Klasse soll eine erste Eigenschaft in Form einer Funktion bekommen. Sind Funktionen Teil einer Klasse, spricht man von einer *Methode*.

```python
class Smiley:
    
    def say_something(self, something):
        print(something)
```

Methoden werden genauso wie Funktionen definiert - einziger Unterschied an dieser Stelle: Als Argument muss immer `self` übergeben werden. `self` steht für eine Instanz der Klasse `Smiley`. Dieses Konzept wird in Kürze deutlicher, wenn wir konkrete Objekte bzw. Instanzen aus der Klasse erstellen.