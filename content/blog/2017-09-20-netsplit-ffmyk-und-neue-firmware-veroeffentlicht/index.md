---
title: "Netsplit Freifunk-MYK und neue Firmware veröffentlicht [Update: Abschaltung altes Netz Feb. 2018]"
date: 2017-09-20T00:00:00+02:00
draft: false
authors:
- nhaerig
timeline: true
---

**Update 19.12.17: Das alte Netz wird am 28.02.2018 abgeschaltet. Router, die bis dahin nicht mit &gt;2017er Firmware aktualierst wurden, gehen offline.**

Im Sommer hatten wir Probleme im Netz. Uplink-Knoten hatten einen dauerhaft hohen Up/Download, Knoten stürzten ab und Nutzer konnten sich nicht mit dem Netz verbinden.

Wir vermuten, dass unser Netz einfach zu groß geworden ist und die kleinen TP-WR841, die wir größtenteils verwenden, damit nicht klar kamen.

Deshalb haben wir im Wiki dem Empfehlung zu diesem Routermodell entfernt (bitte keine neuen mehr kaufen, andere Router z.B. auf TP-WR1043 anschaffen) und unser Netz in Landkreise aufgeteilt. Dazu veröffentlichten wir eine Firmware auf Basis von gluon 2017.1.2. Nach erfolgreichen Tests in Brohl, Mörsdorf, Virneburg und Lahr ist diese nun als Stable eingestuft.

Die neue Firmware ist unter der gewohnten Adresse [https://firmware.freifunk-myk.de/](https://firmware.freifunk-myk.de/) verfügbar.

Allerdings fehlen noch ein paar Services im neuen Netz, wie zum Beispiel die IP-Adressen-Reservierung. Diese werden noch eingebaut.

Das alte Netz wird voraussichtlich noch ein paar Monate laufen. Wenn genügend Router auf das neue Netz gewechselt sind, legen wir eine Deadline zur Abschaltung vom alten Netz fest.** Diese Deadline wird hier im Blog und in der Mailingliste veröffentlicht. Kurz vor der Abschaltung nehmen wir aber bei den fehlenden Knoten Kontakt mit dem Betreiber auf.**

Folgendes ist zu beachten, wenn man die Router updaten will:

 - Router mit neuer Firmware können über WLAN nicht mit Routern alter Firmware meshen.
 - Router, die mit Mesh-On-LAN miteinander verbunden sind erst trennen und dann nacheinander updaten. Ansonsten kann es zu Problemen kommen (Router erhalten IPs aus neuem UND altem Netz).
 - Es besteht keine Verbindung zwischen neuem und altem Netz
 - Der Autoupdater ist standardmäßig aktiviert. Zukünftige stable-releases werden automatisch aktualisert.

Insbesondere bei größeren Installationen mit Fernwartung sollte man darauf achten, sich nicht auszusperren. In Lahr wurden zum Beispiel die meisten Router eingesammelt, aktualisiert und wieder ausgegeben.

EDIT 22.02.18: Die Kontaktaufnahme erfolgte über die eMail-Adresse, die bei der Registrierung vom Nutzer verwendet wurde, nicht über die im Router hinterlegte Kontaktmöglichkeit wie zuerst genannt.
