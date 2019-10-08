# Seed-Test App
Behaviour-driven development (BDD) extends the Test-Driven Development (TDD) approach by the ‘desired behaviour’ of a software. It is designed to ensure a collaboration between business analysts and developers with explicitly written down scenarios. The basic structure for BDD is:

### Loginvorgang
Die benötigten Daten für den Loginvorgang bestehen aus zwei Komponenten – Ihrem GitHub-Namen und dem dazugehörigen GitHub-Account-Token. 
Falls Sie noch keine Token erstellt haben, können Sie diesen in Ihrem GitHub-Profil unter Settings-> Developer Settings-> Personal access tokens-> Generate new token erstellen. Dort werden Sie aufgefordert die Berechtigungen festzulegen, die der Token erteilen kann. Zur Verwendung der CucumberApp benötigt der Key jedoch keine dieser Berechtigungen. 
![alt text](https://github.com/adessoCucumber/Cucumber/blob/master/docs/img1.png "Personal access token")

Nachdem Sie Ihren Benutzernamen und Ihren Token eingegeben haben, können Sie sich in der CucumberApp einloggen.
![alt text](https://github.com/adessoCucumber/Cucumber/blob/master/docs/img2.png "Login")

### Auswahl der Repository
Sobald Sie sich erfolgreich angemeldet haben, können Sie Ihre zu verwendende Repository aus der erscheinenden Liste auswählen.
![alt text](https://github.com/adessoCucumber/Cucumber/blob/master/docs/img3.png "Login Repository")

### Erstellen einer Story
Bevor Sie mit der CucumberApp arbeiten können, müssen Sie ein Issue in Ihrem Repository erstellen und diesem das Label „story“ zuteilen, welches Sie – falls nicht bereits erstellt – zuvor erstellen müssen.
![alt text](https://github.com/adessoCucumber/Cucumber/blob/master/docs/img4.png "Github issue")
![alt text](https://github.com/adessoCucumber/Cucumber/blob/master/docs/img5.png "Github label")
![alt text](https://github.com/adessoCucumber/Cucumber/blob/master/docs/img6.png "Github issue label")
 
### Erstellen/Bearbeiten/Löschen von Szenarios
Sobald Sie Ihre Issues vollständig konfiguriert haben, können Sie in der CumberApp für diese Szenarios erstellen. Hierfür können Sie links für jede Story eine Liste an Szenarios ausklappen. Falls noch kein Szenario existiert, können Sie mit dem „+“-Button ein neues Szenario erstellen. Nachdem Sie ein Szenario erstellt haben, können Sie dies aus der Liste, welche direkt unter dem zuvor erwähnten Button erscheint, auswählen. Bevor Sie dieses Szenario bearbeiten können müssen Sie jedoch den Bearbeitungsmodus aktivieren, wofür Sie den „Lock“- bzw. „Unlock“-Button klicken müssen.
![alt text](https://github.com/adessoCucumber/Cucumber/blob/master/docs/img7.png "Unlock Scenario")

Nachdem Sie den Bearbeitungsmodus aktiviert haben, können Sie das Szenario löschen, den Titel des Szenarios bearbeiten („Pen“-Button neben dem Szenarionamen), den Background des Szenarios festlegen (-> Erklärung in Kapitel „Advanced“) und die Given/When/Then-Elemente ausfüllen bzw. bearbeiten. Für jedes der Given/When/Then-Elemente haben Sie unterschiedliche Möglichkeiten diese zu konfigurieren.  Diese Möglichkeiten können Sie aufrufen und einfügen, indem sie auf den „+“-Button an der rechten Seite des jeweiligen Elementes drücken. Sobald Sie darauf klicken öffnet sich ein kleines Fenster unter dem Button, in welchem Sie verschiedene Auswahlmöglichkeiten haben.
Im Folgenden finden Sie Erklärungen zu den einzelnen Elementen, außerdem eine Auflistung und einzelne Beispiele zu deren Auswahlmöglichkeiten:

1.	Given:
    *	Bezeichnet eine Annahme
    *	Möglichkeiten: Role/Website
    *	Beispiele: “As a XY”, “I am on the website: XY”
2.	When:
    *	Bezeichnet eine Kondition
    *	Möglichkeiten: Website/Button/Field/Radio/Dropdown/HoverOverAndSelect/Checkbox
    *	Beispiele: “I go to the Website: XY”, “I click the button: XY”
3.	Then:
    *	Bezeichnet eine Folge
    *	Möglichkeiten: Website/Text
    *	Beispiele: “So I will be navigated to the website: XY”, “So I can see the text XY in the textbox: XY”

![alt text](https://github.com/adessoCucumber/Cucumber/blob/master/docs/img8.png "Edit scenario")

Sobald Sie alle Elemente erstellt und korrekt ausgefüllt haben, können Sie mit dem zuvor erwähnten „Lock“- bzw. „Unlock“-Button den Bearbeitungsmodus wieder verlassen.

### Durchführen von Test und Abspeichern der Testdaten
Da Sie nun ein Szenario konfiguriert haben, können Sie für dieses Tests durchführen. Dazu können Sie den „Run Tests“-Button, welcher sich direkt unter dem „Example“-Feld befindet, verwenden. Sobald Sie diesen drücken, werden Tests mit Ihren zuvor festgelegten Vorgaben (given/when/then) durchgeführt. Sind die Tests alle beendet, werden Ihnen die Ergebnisse in einer Übersicht dargestellt.
![alt text](https://github.com/adessoCucumber/Cucumber/blob/master/docs/img9.png "Test report")

Außerdem haben Sie die Möglichkeit sämtliche Metadata durchzulesen und sich unter „Features“ alle auftretenden Fehler zusammen mit deren Fehlermeldungen durchzulesen. 
![alt text](https://github.com/adessoCucumber/Cucumber/blob/master/docs/img10.png "test report details")

Neben dem „Run Tests“-Button wurden nun zwei weitere Buttons freigeschaltet, der „Pfeil“-Button, welchen Sie verwenden können, um das Testergebnis-Feld einzuklappen und auch wieder auszuklappen, und der „Download“-Button, über welchen Sie Ihre Testergebnisse herunterladen können.
Sie haben außerdem die Möglichkeit Test für alle von Ihnen erstellte Szenarios auszuführen. Hierfür können Sie den „Run Story“-Button verwenden. Der Ablauf der Tests erfolgt exakt so wie der Test eines einzelnen Szenarios. Sie können nun in der Anzeige der Testergebnisse unter „Feature“ eine Auflistung aller getesteter Szenarios finden und diese auf mögliche Fehlermeldungen untersuchen. Auch diese Ergebnisse können Sie unter Verwendung des „Download“-Buttons herunterladen.

### Advanced
In diesem Kapitel finden Sie nützliche Aktionen, die Sie neben den Hauptaktionen verwenden können.
1.	Background:
    *	Den Background können Sie verwenden, um gleiche Given-Statements in mehreren Szenarios zu verwenden. Der Background wird vor jedem Szenario, welches diesen verwendet, ausgeführt.
    *	Beispiel:
    ![alt text](https://github.com/adessoCucumber/Cucumber/blob/master/docs/img11.png "Background")
2.	Examples:
    *	Zur Verwendung von Examples können Sie in ihren Given/When/Then-Statements Platzhalter erstellen. Diesen können Sie in einer Tabelle Werte zuweisen, welche an Stelle des Platzhalters verwendet werden. Einem Platzhalter können mehrere Werte zugewiesen werden. Ist dies der Fall, werden alle Werte nacheinander in diesen Platzhalter eingesetzt und Tests mit ihnen durchgeführt.
    *	Beispiel: 
    ![alt text](https://github.com/adessoCucumber/Cucumber/blob/master/docs/img12.png "Examples")

### Nützliche Links
In diesem Kapitel finden Sie eine Auflistung nützlicher Links, welche bei Problemen helfen sollen.
* [Gherkin](https://cucumber.io/docs/gherkin/reference/)
* [BDD](https://cucumber.io/docs/bdd/)
* [Cucumber](https://cucumber.io/docs/cucumber/)


### License

Copyright (c) 2018 Adesso AG Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
