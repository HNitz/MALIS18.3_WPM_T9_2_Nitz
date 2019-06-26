## Ziel

Es soll ein internes Tool erstellt werden, mit dem sich die Einhaltung der neuen Datenschutz-Grundverordnung effizient und 
zeitsparend umsetzen lässt. Derzeit müssen von allen Projektteams Verfahrensbeschreibungen für die Verarbeitung persönlicher 
Daten erstellt werden, z.B. der Zuwendungsempfänger/-Innen, Teilnehmer/-Innen, Gutachter/-Innen, Dolmetscher/-Innen usw. 
Die einzelnen Quell-Datenbanken sind zu komplex, nicht alle Mitarbeiter/-Innen sind damit vertraut. Außerdem ist die ständige 
manuelle Prüfung der zu löschenden Daten mit einem hohen Aufwand verbunden und sehr fehlerbehaftet. 
Daher soll ein Lösch-Tracker erstellt werden, der auf die Informationen in allen Datenbanken zugreift und die Mitarbeiter/-Innen 
an die fristgemäße Löschung personenbezogener Daten erinnert, wenn die automatisch erkannte Frist für das Projektende und das 
Ablaufen der Aufbewahrungspflicht eintritt. Dabei gibt es verschiedene Kategorien von Daten. Nicht mehr benötigte Daten 
(z.B. Geburtsdaten, Reisepass-Nummern,…) müssen unmittelbar nach der Beendung einer Aktivität gelöscht werden. Zahlungsrelevante 
Daten müssen zum Zweck der Rechnungsprüfung für eine Dauer von 10 Jahren archiviert werden. Darüber hinaus kann die Zustimmung 
zur Speicherung inhaltlich relevanter Daten, z.B. Kontaktinformationen und Fachexpertise, bei den betreffenden Personen abgefragt 
werden, sodass diese Daten zum Zweck zukünftiger Aktivitäten erhalten bleiben.


## Vorgehen / Plan für Code

Import von Daten aus SQL- und Access-Datenbanken

Liste generieren: alle Projekte werde mit Auslaufdatum in chronologischer Reihenfolge angezeigt

Code erkennt automatisch anhand des hinterlegten Datums für das Projektende, welche Datensätze gelöscht werden müssen

alle zu löschenden Datensätze werden rot und als "Projektdauer abgelaufen, Löschen erforderlich" angezeigt 

Mitarbeiter wird zum Autorisieren der Löschung aller betroffenen Datensätze aufgefordert 

Datensatz wird mit Meldung "gelöscht" und Datum der Löschung gekennzeichnet
