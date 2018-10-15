<h1 class="norm">FAIRly SUSTAINABLE RESEARCH SOFTWARE?</h1>

Stephan Druskat, ORCID [0000-0003-4925-7248](https://orcid.org/0000-0003-4925-7248)

Developer Forum der Humboldt-Universität, 15. Okt. 2018

Folien: https://sdruskat.net/hu-dev-forum-2018/

Note:
Naiveté, regression, despair


## About

- Magister Anglistik, Linguistik, neuere dt. Literatur
- seit 2008: Softwareentwicklung in der Forschung
- <span class="fragment highlight-red">Research Software Engineer (RSE)</span>, Inst. f. dt. Sprache und Linguistik
- Mitbegründer [de-RSE](https://de-rse.org/)
- [Special Collaborator](https://fellows.software.ac.uk/) des [Software Sustainability Institute](https://www.software.ac.uk/)
- Forschungsinteressen: Nachhaltigkeit von Forschungssoftware, Softwarezitierung


## Research Software Engineer?

<ul class="fragment fade-in">
<li>Softwareentwickler mit Domänenwissen</li>
<li>Softwaretechnik > (Nach-)nutzbarkeit, "Korrektheit"</li>
<li>Sichtbarkeit des Tätigkeitsfeldes</li>
</ul>

<ul class="fragment fade-in">
<li>[Vereinsgründung *de-RSE e.V. - Gesellschaft für Forschungssoftware*](https://www.de-rse.org/de/association.html): 26.11.2018</li>
<li>Konferenz [*#deRSE19*](https://www.de-rse.org/de/conf2019/index.html): 4.-6.6.2019, Potsdam</li>

Note:
- Personen, die in der Wissenschaft arbeiten und Software entwickeln.
- wenden Methoden aus der Softwaretechnik auf Forschungssoftware an
- verbinden sie Wissen aus der Softwareentwicklung mit Domänenwissen
- sorgen so dafür, dass die entstehende Forschungssoftware nutzbar und nachnutzbar ist und nachvollziehbar korrekte Forschungsergebnisse liefert
- Bei dem Begriff geht es aber auch um die Sichtbarkeit des Tätigkeitsfeldes, Softwareentwicklung in der Wissenschaft



## Forschungssoftware? 

DFG:

> Eigens zum wissenschaftlichen Erkenntnisgewinn erstellte Software-Anwendungen und Software-Bibliotheken

Note:
- Skripte
- komplexe Anwendungen



## Wozu nachhaltige Forschungssoftware?

- Reproduzierbarkeit von Forschungsergebnissen.

Zentrale Frage:

### Wie Forschungssoftware nachhaltig entwickeln?

Note:
- Forschungsdaten und darauf beruhende Forschungsergebnisse sind ohne Überprüfbarkeit
der Methode durch die sie erlangt oder analysiert worden sind nicht stichhaltig
zu evaluieren.
- Zentrale Frage: ich kann keine zentrale Antwort geben, sondern werde vor allem
viele Folgefragen stellen, die wir im Anschluss diskutieren sollten



## Nachhaltige Forschungssoftware? 

> Nachhaltigkeit ist die Fähigkeit einer Software, Bestand zu haben, also
zukünftig verfügbar zu sein, auch auf neuen Plattformen, und neuen Bedürfnissen
gerecht zu werden.  
[Daniel S. Katz](https://danielskatzblog.wordpress.com/2016/09/13/defining-software-sustainability/)

- Viele Aspekte
- [Viele Blickwinkel](https://danielskatzblog.wordpress.com/2018/09/26/fundamentals-of-software-sustainability/)
- Realität?

Note:
- keine operationalisierbare Definition um das Konzept zu verstehen
- verschiedene Stakeholder: veschiedene Definitionen

- *User:* Shoppingliste mit Aspekten der Langlebigkeit
- *Förderer:* Portfolio Management: Investition in potenziell erfolgreiche Projekte
- *Forschungsmanager*: Fokus auf Menschen (Human Resources), also wie Business Management
- *Entwickler:* Fokus auf Ressourcen, um a) die Software langlebig zu machen und b) um sich selbst zu verstetigen

Aspekte:
- technische Nachhaltigkeit (SE, Containerisierung, Langzeitverfügbarkeit, Ökosysteme)
- personelle Nachhaltigkeit
- Kreditabilität und Attribution (Nachvollziehbarkeit)
- Nachhaltigkeit des Wissens: Dokumentation!

Die Realität von Softwareentwicklung in der Wissenschaft steht dem gebenüber.



<h2 class="norm">FAIRe Software?</h2>

- Modell Forschungsdaten: [**F**indable, **A**ccessible, **I**nteroperable, **R**eusable](http://www.forschungsdaten.org/index.php/FAIR_data_principles)
- FAIR-Prinzipien bestehen nur auf Zugänglichkeit der Metadaten
- Credit (Anerkennung) spielt keine Rolle
- [FORCE11 Scholarly Commons WG](https://www.force11.org/group/scholarly-commons-working-group): "Open, FAIR, citable"
- https://danielskatzblog.wordpress.com/2017/06/22/fair-is-not-fair-enough/

Note:
- Zugänglichkeit der Metadaten nicht ausreichend
- Credit ist unumngänglich um personelle Nachhaltigkeit zu gewährleisten
- zur Realität von Auffindbarkeit komme ich gleich noch



<h2 class="norm">Faire (auffindbare) Software: Softwarezitierung</h2>

<table>
<tr>
<td style="vertical-align: top;">
<ul>
<li>Anerkennung/Zuschreibung für Software?</li>
<li>Systeme für Softwarecredit?</li>
<li>Wie wird Software zitiert?</li>
</ul>
</td>
<td>
<img src="table.png" style="width: 200%;">

[10.7717/peerj.2394/table-1](https://doi.org/10.7717/peerj.2394/table-1)
</td>
</tr>
</table>

Note:
- Wie kann Auffindbarkeit und Zuschreibung funktionieren?
- Neues System oder Piggybacking auf existierendes System


## Citation File Format

- [Format für Softwarezitierungsmetadaten](https://citation-file-format.github.io/), `CITATION.cff`
- Entwicklung beim [WSSSPE5.1-Workshop](https://www.software.ac.uk/blog/2017-12-12-standard-format-citation-files), [Druskat et al. (2018): CFF 1.0.3](https://doi.org/10.5281/zenodo.1405679)

```yaml
cff-version: 1.0.3
message: "If you use this software, please cite it as below."
authors:
  - family-names: Druskat
    given-names: Stephan
    orcid: "https://orcid.org/0000-0003-4925-7248"
title: My Research Tool
version: "1.0.4"
doi: "10.5281/zenodo.1234"
date-released: 2017-12-18

```

> Druskat, Stephan (2017). My Research Tool (Version 1.0.4). DOI: 10.5281/zenodo.1234.



## Best practices

- Software Engineering!
- Institutionsleitlinien (z.B. [Deutsches Zentrum für Luft- und Raumfahrt](https://doi.org/10.5281/zenodo.1344608))
- ["Handreichung zum Umgang mit Forschungssoftware"](https://doi.org/10.5281/zenodo.1172970)
- HU?

Note:
- Im Prinzip muss man die Gesamtheit des State of the Art des Software Engineering anwenden
- "Allianz der deutschen Wissenschaftsorganisationen"
- es gibt viele Best Practices
- Open Access-Erklärung erwähnt Software nicht
- Für eingebettete RSEs in kleinen Projekten ist das oft aber kaum zu schaffen, es sei denn, sie haben entsprechende Vorbildung und Fokus.



## "Good enough practices in scientific computing" ([Wilson et al. 2017](https://doi.org/10.1371/journal.pcbi.1005510))

> Place a brief explanatory comment at the start of every program.


### "Good enough practices in scientific computing" ([Wilson et al. 2017](https://doi.org/10.1371/journal.pcbi.1005510))

> Decompose programs into functions.


### "Good enough practices in scientific computing" ([Wilson et al. 2017](https://doi.org/10.1371/journal.pcbi.1005510))

> Be ruthless about eliminating duplication.


### "Good enough practices in scientific computing" ([Wilson et al. 2017](https://doi.org/10.1371/journal.pcbi.1005510))

> Always search for well-maintained software libraries that do what you need.


### "Good enough practices in scientific computing" ([Wilson et al. 2017](https://doi.org/10.1371/journal.pcbi.1005510))

> Test libraries before relying on them.


### "Good enough practices in scientific computing" ([Wilson et al. 2017](https://doi.org/10.1371/journal.pcbi.1005510))

> Give functions and variables meaningful names.


### "Good enough practices in scientific computing" ([Wilson et al. 2017](https://doi.org/10.1371/journal.pcbi.1005510))

> Make dependencies and requirements explicit.


### "Good enough practices in scientific computing" ([Wilson et al. 2017](https://doi.org/10.1371/journal.pcbi.1005510))

> Do not comment and uncomment sections of code to control a program's behavior.


### "Good enough practices in scientific computing" ([Wilson et al. 2017](https://doi.org/10.1371/journal.pcbi.1005510))

> Provide a simple example or test data set.


### "Good enough practices in scientific computing" ([Wilson et al. 2017](https://doi.org/10.1371/journal.pcbi.1005510))

> Submit code to a reputable DOI-issuing repository.


### "Good enough practices": Documentation

1.	<span style="color: red;">Place a brief explanatory comment at the start of every program.</span>
2.	Decompose programs into functions.
3.	Be ruthless about eliminating duplication.
4.	Always search for well-maintained software libraries that do what you need.
5.	<span style="color: red;">Test libraries before relying on them.</span>
6.	<span style="color: red;">Give functions and variables meaningful names.</span>
7.	<span style="color: red;">Make dependencies and requirements explicit.</span>
8.	Do not comment and uncomment sections of code to control a program's behavior.
9.	<span style="color: red;">Provide a simple example or test data set.</span>
10.	Submit code to a reputable DOI-issuing repository.

Note:
- Die Hälfte der obigen Punkte bezieht sich unter anderem auf Dokumentation.
- Dokumentation ist in der Tat der offensichtliche Weg, um überhaupt erst ein Potenzial der Software für Nachhaltigkeit zu schaffen.
- Folgerichtig wäre also eine wichtige Handlungsanweisung für Softwareentwickler in der Wissenschaft diese:


## Document All The Things!!1!11ELF(?)

<img src="doc.png" style="width:60%">

Note:
- Wie realistisch ist das?



## Good enough practices (of documentation)

- "Brief explanatory comment at the start of every program"?
- Was dokumentieren?
- Wie tief dokumentieren?
- Wie breit dokumentieren?
- Wie meta dokumentieren?
- In welcher Form dokumentieren?

Note:
- Ist ein "Brief explanatory comment at the start of every program" genug?
- Wie tief muss die Dokumentation gehen? Bis auf einzelne Schritte in Algorithmen?
- Wie breit muss die Dokumentation angelegt sein? Muss Verhalten der Abhängigkeiten mit dokumentiert sein?
- Wie meta muss Dokumentation sein? Müssen Designentscheidungen, etc., mit dokumentiert sein? Auch die Entscheidung, wie und was dokumentiert werden soll? Müssen Contribution-Workflows dokumentiert sein, vielleicht sogar Communityregeln?
- Welche Form muss die Dokumentation haben? API-Docs, Codekommentare? Fließtext? Integrierte Dokuemntation? Wikis? README?
- Wie sollte die Dokumentation erreichbar sein? GitHub README? Zitierfähige Publikation? Software-Metapaper?


## Realistic practices (of documentation)?

Note:
- was davon können wir überhaupt schaffen? Was davon müssen wir schaffen?
- Antwort: Es kommt darauf an! Und zwar auf das Projekt.
- Bei Skripten von unter 100 Zeilen reicht vielleicht ein Kommentar oben im Quelltext. 
- Bei Skripten von über 100 oder 1000 Zeilen vielleicth nicht mehr? 
- Und sollten diese nicht sowieso in Module geteilt werden?
- GUI-Applikationen bedürfen anderer "interner" Dokumentation als Kommandozeilen-Skripte, die interaktiv durch die Bedienung leiten können oder man-pages haben.
- Das *Zielpublikum* spielt immer eine Rolle, d.h., welche Nutzer brauchen welche Art von Dokumentation?
- Welche Art von Dokumentation erwarten Entwickler? Java-Entwickler erwarten vielleicht Javadoc und API-Docs, usw.



# Danke!

- **Software Sustainability Institute**: EPSRC, BBSRC, ESRC Grant EP/N006410/1
- **Projektförderung:** DFG grant GA 1288/11 ("Research software sustainability")

Folien: https://sdruskat.net/hu-dev-forum-2018

stephan.druskat@hu-berlin.de, <i class="fa fa-twitter"/></i> [@stdruskat](https://twitter.com/stdruskat),
<i class="fa fa-github"/></i> [@sdruskat](https://github.com/sdruskat)
