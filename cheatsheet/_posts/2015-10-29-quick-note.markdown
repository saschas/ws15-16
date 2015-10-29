---
layout: post
title:  "Quick note: main.css ändern"
date:   2015-10-29 21:15:00
categories: admin
---

# Hilfe: Meine Änderungen in der main.css ändern nichts

Danke @henningxx für den Hinweis!
Scheinbar haben einige von euch Probleme beim Ändern der Stylesheets. 
Ich weiß nicht genau woran es liegt, aber ich habe eine _Ahnung_.
Für diejenigen bei denen das Problem auftritt:

1. Öffnet die DevTools mit cmd-alt-i oder _Anzeigen_ > _Entwickler_ > _Entwicklertools_
2. Switched in den _Source Tab_
![Source Tab Chrome DevTools]({{ site.url }}/assets/img/source_tab.png)
3. Ordner per _drag&drop_ auf das Fenster ziehen und anschließend __Zugriff erlauben__
![Source Tab Chrome DevTools]({{ site.url }}/assets/img/drag_n_drop.gif)
4. Öffnet den Ordner _initializr_ > _css_ in den DevTools
5. Zum testen könnt ihr ja mal versuchen die Hintergrundfarbe zu ändern:
   
{% highlight css %}
    body{
      background:red;
    }
{% endhighlight%}

__Sollte das nicht funktionieren__ kann es sein das ihr den falschen Ordner geöffnet habt.
Wenn ihr die Seite von eurem lokalen Server aus aufruft, also z.B. `http://localhost:8080/` seht ihr wahrscheinlich in eurem Source Tab gleich mehrere Ordner.

Vergewissert euch das ihr in eurem __lokalen__ Ordner (hier grün) arbeitet und __nicht__ in dem (hier roten) Ordner. Ihr könnt euch sicher sein das es der richtige Ordner ist wenn ihr ein _Ordnericon_ vor dem Namen seht und _keine_ Weltkugel.

![Source Tab Chrome DevTools]({{ site.url }}/assets/img/ordner_in_source_tab.png)

Ich hoffe das hilft euch erstmal weiter, falls ihr weitere Fragen habt oder an dieser Stelle nicht weiterkommt schreibt mich einfach über mein Mail(sigl@htw-berlin.de) an oder über den Twitter Account(@ws15_16).

Viel Spaß beim coden!

---

#### Mehr Tips zu den Chrome DevTools
- [Tips zu den Chrome DevTools](https://developer.chrome.com/devtools/docs/dom-and-styles?hl=fi)
- [Inspect and Tweak Your Pages: the Basics](https://developers.google.com/web/tools/chrome-devtools/iterate/inspect-styles/basics?hl=en)
- Video:[Wait, Chrome DevTools can do THAT](https://www.youtube.com/watch?v=BaneWEqNcpE)