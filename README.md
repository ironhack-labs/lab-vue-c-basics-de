![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# LAB | Vue.js Basics (Composition API)

## Einführung


In diesem Lab wirst Du die Grundlagen von Vue.js erkunden und die Grundlage für größere und kompliziertere Projekte schaffen.

Das sind die Aufgaben, die Du in diesem Lab erledigen wirst:

- Erstellen einer grundlegenden Template-Struktur innerhalb eines neuen Projekts.
- Anzeige des Ergebnisses einer JavaScript-Operation im HTML einer Komponente.
- Anzeige eines Elements nur dann, wenn eine bestimmte Eigenschaft auf "true" gesetzt ist.
- Anzeige einer Liste von Elementen, die in einer Komponente gespeichert sind.
- (Bonus) Änderung der Hintergrundfarbe eines Elements beim Drücken eines Buttons.

Lass uns beginnen!

## Anforderungen

-   Fork dieses Repo
-   Clone dieses Repo
-   Öffne das LAB und starte:

  ```bash
  $ cd lab-vue-basics
  $ npm install
  $ npm run dev
  ```

## Abgabe

- Nach Abschluss führe folgende Befehle aus:

  ```bash
  git add .
  git commit -m "done"
  git push origin main
  ```

- Erstelle einen Pull-Request, damit Deine TAs Deine Arbeit überprüfen können.


<!-- ## Getting Started -->  



## Anleitung

### Iteration 1 | Erstelle eine grundlegende Vorlagenstruktur in einem neuen Projekt

Für dieses Labor musst Du ein neues Vue-Projekt in einem neuen Ordner erstellen. Du kannst entscheiden, welche Optionen Du einbeziehen möchtest.

Einer der Hauptvorteile von Vue (oder jedem anderen Frontend-Framework) besteht darin, wie einfach es ist, Komponenten in Deiner gesamten Anwendung wiederzuverwenden. Das ist genau das, was wir jetzt üben werden.

Du musst eine `navbar`-Komponente und eine `footer`-Komponente erstellen, die Du in allen inneren Seiten Deiner App einbeziehst. Hinweis: Wenn Du sie in Deiner App.vue-Komponente importierst, werden sie auch auf all Deinen inneren Seiten angezeigt.

Im Moment musst Du Dich nicht um das Styling dieser Komponenten kümmern. Stelle einfach sicher, dass sie funktionieren und Du kannst zur nächsten Aufgabe übergehen.



### Iteration 2 | Das Ergebnis einer JavaScript-Operation in HTML eines Komponenten anzeigen

Du hast bereits geübt, wie man eine `string` innerhalb eines Vue-Komponenten-Templates mit Hilfe der Mustache-Syntax (`{{}}`) anzeigt. Du hast auch gesehen, dass Zeichenfolgen nicht die einzigen Dinge sind, die man auf HTML mit dieser Technik einfügen kann.

Diese Herausforderung besteht aus zwei Teilen:

- Zunächst müssen Sie einfach eine mathematische Operation in Ihr HTML einfügen und sehen, was passiert. Etwas so Einfaches wie `2 + 2` ist hier ausreichend.
- Dann beginnt die eigentliche Herausforderung: Sie müssen eine `string` in Ihrem Template "drucken", jedoch mit einem Kniff: Diese Zeichenfolge muss von einer Funktion zurückgegeben werden  und die in anderen reaktiven Variablen gespeicherten Daten lesen. Hinweis: [Dieser Artikel](https://lavalite.org/blog/created-and-mountedin-vuejs) kann Ihnen helfen, zu verstehen, wie Sie dies tun können.


### Iteration 3 | Zeige ein Element nur dann an, wenn eine bestimmte Eigenschaft auf `true` gesetzt ist

Einer der Hauptgründe, warum wir etwas wie Vue verwenden, ist die Vereinfachung gängiger JavaScript-Operationen. Einer der Hauptvorteile dieses Frameworks ist, dass es uns auf sehr einfache Weise ermöglicht, Elemente bedingt anzuzeigen.

Lassen Sie uns das üben! Deine Herausforderung hier besteht darin, eine boolesche Daten innerhalb eines Vue-Komponenten zu erstellen und es mit einem HTML-Element zu verknüpfen, das nur in deinem Template angezeigt wird, wenn die Bedingung auf `true` gesetzt ist.

Wir haben heute die `v-if` und `v-show` Eigenschaften in der Klasse gesehen; aber wenn du feststeckst, kann [die offizielle Dokumentation](https://v2.vuejs.org/v2/guide/conditional.html) hier sehr hilfreich sein. Denken Sie auch daran, dass der boolesche Wert in Ihrem `<script setup>` definiert werden muss.

### Iteration 4 | Zeige eine Liste von Elementen an, die innerhalb eines Komponentenobjekts gespeichert sind

Erinnerst du dich, wie schwierig `for-Schleifen` in Vanilla JavaScript zu sein schienen? Vue erleichtert uns einiges, wenn wir sie verwenden, und ermöglicht es uns, eine Liste von Elementen auf dem Bildschirm auf eine viel einfachere Weise anzuzeigen.

In dieser Übung wirst du üben, wie man die `v-for`-Direktive verwendet. Die Herausforderung besteht aus den folgenden Komponenten:

-   Du musst eine Liste von Posts als `ref()` einer deiner Vue-Komponenten erstellen. Diese Posts müssen folgende Daten enthalten: Titel, Beschreibung und Inhalt; und du benötigst mindestens drei von ihnen.
-   Dann musst du die Posts auf deinem `template` mit Hilfe der `v-for`-Direktive "anzeigen".

Wenn du hier feststeckst, [kannst du immer auf die offizielle Dokumentation verweisen](https://v2.vuejs.org/v2/guide/list.html).


### Iteration 5 | Bonus | Ändere die Hintergrundfarbe eines Elements beim Drücken eines Buttons

Bereit für eine schwierigere Herausforderung? Mit Vue können wir ziemlich "magische" Dinge auf einfache Weise tun. In diesem Fall lernst du, wie du eine CSS-Eigenschaft dynamisch ändern kannst, indem du Daten binden.

Wir sind nicht sehr tief in dieses Thema eingestiegen, aber hier sind einige Tipps, die dich in die richtige Richtung weisen:

-  Du musst entweder eine Klasse oder eine CSS-Eigenschaft erstellen und sie an eine Bedingung [binden](https://v1.vuejs.org/guide/syntax.html).
-  Du musst eine Methode erstellen, die die Klasse oder die Eigenschaft ändert, und sie über einen Klick auf einen Button auslösen. Das ist etwas, was wir noch nicht behandelt haben, aber versuche, Online-Ressourcen zu nutzen, um herauszufinden, wie es gemacht wird. Hier sind einige Links, um dir in die richtige Richtung zu helfen:
  - [Vue.js - Class and style binding](https://vuejs.org/guide/essentials/class-and-style.html)
  - [Stack Overflow](https://stackoverflow.com/questions/59354679/add-background-color-when-click-a-button-vue-js)

Klingt gut? Dann lasst uns loslegen!

<br>

**Viel Spaß beim Coden!** :heart: