---
title: "Workaround Meshverlust Nodes"
date: 2016-10-23T00:00:00+02:00
draft: false
authors:
- nhaerig
timeline: false
---

#### **Problem**

Seit einiger Zeit beobachte ich bei einem TP-Link TL-WR841 v9 mit gluon-v2016.1.5, der als Relais dient, folgende Anomalie:

Der Router steigt aus und wird auf der Karte als offline angezeigt. Andere Nodes bauen keine Verbindung zu ihm auf. Nach ~15 Stunden kommt er wieder online und alles ist OK. Uptime sagt, dass Router die ganze Zeit eingeschaltet war.

Ein Mitfunker gab mir den Tipp, einen Cronjob anzulegen, der den Router ein Mal pro Stunde neu startet. Das erscheint mir ein wenig übers Ziel hinaus zu schießen, also habe ich ein Skript geschrieben, das ein Mal pro Stunde den nächsten Node anpingt und bei dreimaligem Misserfolg das Netzwerkmodul neu startet. Zwischen zwei Versuchen macht das Skript eine Minute Pause.

Ergebnisse werden in /tmp/mesh_check.log gespeichert.

Das Skript ist jetzt im Testbetrieb. Verbesserungsvorschläge implementiere ich gerne :)

#### **Installation**

Skript in z.B. /opt/mesh_check.sh einfügen

Skript mit „chmod +x /opt/mesh_check.sh“ ausführbar machen

Cronjob anlegen mit „crontab -e“ und dann „0 0 * * * /opt/mesh_check.sh“ einfügen, damit Skript ein Mal pro Stunde ausgeführt wird.

#### **Skript**

[https://github.com/GitNorb/mesh_check](https://github.com/GitNorb/mesh_check)

EDIT: Skript auf GitHub umgezogen

