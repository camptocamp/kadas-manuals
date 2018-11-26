<!-- WARNING: This file is autogenerated by csv2md.py -->
# KADAS Benutzeroberfläche

<img src="../media/image1.png" />

Die KADAS Benutzeroberfläche ist in fünf Bereiche unterteilt:

+ Funktionsmenü
+ Favoriten und Suche
+ Kartenfenster
+ Ebenen und Geodatenkatalog
+ Status Bar


## <a name="sec0"></a>Funktionsmenü

Im Funkionsmenü kann über eine Menüleiste zwischen verschiedenen Symbolleisten umgeschaltet werden. Die Symbolleisten enthalten Knöpfe für die verschiedenen Funktionen. Die Funktionen der Symbolleisten sind in separaten Kapiteln dokumentiert:

+ Meine Karten
+ Ansicht
+ Analyse
+ Zeichnen
+ GPS
+ MSS
+ Einstellungen / Hilfe


## <a name="sec1"></a>Favoriten und Suche

### Favoriten

Auf den vier Platzhaltern können favorisierte Funktionen aus dem Funktionsmenü platziert werden. Dies geschieht durch Ziehen der Maus bei gedrückter Maustaste. Der Favorit kann durch Drücken der rechten Mausstaste wieder entfernt werden. Die Favoriten werden als Benutzereinstellungen gespeichert.


### Suche

Das Suchfeld bietet eine einheitliche Schnittstelle für verschiedene Suchdienste:

+ Koordinaten (LV03, LV95, DD, DM, DMS, UTM, MGRS)
+ Ortschaften und Adressen schweizweit
+ Ortschaften weltweit
+ Attribute in lokale Datensätze
+ Attribute in remote Datensätze (Web-Dienste)
+ Attribute in Stecknadeln

Nach der Eingabe von mindestens drei Buchstaben startet die Suche und es werden erste Resultate angezeigt.

Die Resultate werden in entsprechend bezeichnete Kategorien aufgelistet. Die Resultatliste kann mit Maus oder Tastatur-Pfeile durchsucht werden. Beim Auswählen eines Resultats mit den Pfeilen wird eine blaue Stecknadel an den entsprechenden Ort gesetzt. Beim aktivieren eines Resultats mit der Maus wird der Kartenausschnitt auf den entsprechenden Ort zentriert.

<img src="../media/image2.png" />

Rechts vom Suchfeld gibt es die Möglichkeit, einen Filter für die lokale und remote Datensatz-Suche zu definieren. Dieser Filter greift nicht für Koordinaten, Ortschaft oder Stecknadelsuchen.


## <a name="sec2"></a>Kartenfenster

Dies ist der Ergebnisbereich von KADAS - hier werden die Daten visualisiert. Die Karten, die hier angezeigt werden, hängen davon ab, welche Raster- und Vektorlayer Sie ausgewählt haben.

Innerhalb des Kartenfensters können Sie ‘zoomen’, verschieben und eine Vielzahl weiterer Funktionen aus der Werkzeugleiste anwenden. 

Das Kartenfenster und die Legende sind miteinander verknüpft. Layer im Kartenfenster spiegeln Veränderungen in der Legende wider.

In der Registerkarte Ansicht können neue Kartenunterfenster geöffnet werden. 


## <a name="sec3"></a>Ebenen und Geodatenkatalog

Am linken Rand des Programmfensters befindet sich ein aufklappbarer Bereich, welche Verwaltungsfunktionen für Kartenebenen enthält. Im oberen Teil ist die Kartenlegende und im unteren Teil der Geodatenkatalog angeordnet.


### Ebenen

Der Bereich der Kartenlegende verzeichnet alle **_Ebenen_** des Projekts. Das Kontrollkästchen für jedes Element der Legende kann benutzt werden, um die Ebene ein- oder auszublenden.

Die Z-Anordnung der Kartenlayer kann mit der ‘drag and drop’ Funktion der Maus festgelegt werden. Z-Anordnung bedeutet, dass ein weiter oben in der Legende angeordneter Layer über einem weiter unten angeordneten Layer im Kartenfenster angezeigt wird.

Die Ebenen im Legendenfenster können als Gruppen organisiert werden.

Um einen Layer aus einer Gruppe zu bringen, können Sie ihn herausschieben oder einen Rechtsklick darauf machen und **_In oberste Ebene bringen_** wählen. Gruppen können auch in andere Gruppen verschachtelt werden.

Das Kontrollkästchen für eine Gruppe zeigt oder verbirgt alle Layer einer Gruppe mit einem Klick.

Bei einem Rechtsklick hängt das Kontextmenü davon ab, ob es sich beim ausgewählten Element in der Legende um eine Raster- oder Vektor-Ebene handelt.

+ **Rechte-Maustaste-Menü für Rasterlayer**
  + Zoom to Layer
  + Entfernen
  + Kopieren
  + Eigenschaften...
+ **Rechte-Maustaste-Menü für Vektorlayer**
  + Zoom to Layer
  + Entfernen
  + Kopieren
  + Eigenschaften...
+ **Rechte Maustaste-Menü für Layergruppen**
  + Entfernen
  + Umbenennen

Es ist möglich mehr als einen Layer oder Gruppe zur gleichen Zeit auszuwählen indem man die Strg Taste gedrückt hält und die Layer mit der linken Maustaste auswählt. Sie können dann alle ausgewählten Layer gleichzeitig zu einer neuen Gruppe verschieben.


### Geodatenkatalog

Im Geodatenkatalog können weitere Kartenebenen zur Karte hinzugefügt werden. Ist die Liste leer, besteht keine Netzwerkverbindung zum Katalogdienst. Durch Eingabe von Suchbegriffen im Textfeld werden die verfügbaren Ebenen entsprechend eingeschränkt. Eine Ebene kann mittels Kontextmenü (rechte Maustaste auf dem Ebeneneintrag) oder via “Drag and Drop” der Karte hinzugefügt werden.

Oberhalb der Katalogliste stehen folgende Funktionen zur Verfügung:

+ **_Lokaler Datensatz hinzufügen_**: Es können Vektordaten oder Rasterdaten zur Karte hinzugefügt werden.
+ **_Katalog neu laden_**: Lädt die Liste der verfügbaren Kartenebenen neu.
+ **_SAML Authentifizierung_**: Es wird ein Fenster geöffnet, in dem ein webbasiertes Login auf dem Server durchgeführt werden kann. Nach erfolgreichem Login wird der Geodatenkatalog neu geladen und es stehen entsprechend den Berechtigungen zusätzliche Kartenebenen zur Verfügung.


## <a name="sec4"></a>Statusbar

In der Statuszeile sind folgende Anzeigen und Bedienelemente angeordnet:

+ **GPS**: Die Funktion des GPS-Knopfes ist unter "GPS aktivieren beschrieben".
+ **Mausposition**: Die aktuelle **_Mausposition_** kann in verschiedenen Koordinatensystemen angezeigt werden. Das gewünschte Anzeigesystem kann über den Knopf rechts der Positionsanzeige ausgewählt werden.
+ **Massstab**: Neben der Koordinatenanzeige finden Sie die **_Massstabsanzeige_**. Es zeigt den Massstab des Kartenfensters. Wenn Sie herein- oder hinauszoomen zeigt KADAS ihnen den aktuellen Maßstab. Es gibt eine **_Massstabsauswahl_** mit der Sie zwischen vordefinierten Massstäben von 1:500 bis 1:1000000 wählen können.
+ **Koordinatensystem**: Im Auswahlfeld **_Koordinatensystem_** kann das Referenzsystem ausgewählt werden, in dem die aktuelle Karte dargestellt werden soll. Das angzeigte Referensystem kann vom Referenzsystem, in dem die Daten vorliegen, abweichen. In diesem Fall werden die Daten zur Darstellung umprojiziert.
