# auto-schluessel

Liefert unter `https://auto.lukaspriess.de/.well-known/appspecific/com.tesla.3p.public-key.pem`
den öffentlichen Schlüssel aus, den Tesla für die Anbindung des eigenen Fahrzeugs an das
Dashboard verlangt (Fleet API). Sonst nichts: keine Anwendung, keine Daten, keine Verbindung
zum Dashboard.

- Ausgeliefert von GitHub Pages aus dem Branch `seite`; `CNAME` nennt die Adresse, `.nojekyll`
  lässt den Ordner `.well-known` durch.
- Der private Schlüssel liegt nur auf dem Server des Dashboards und nie in einem Repo.
- Wird dieses Repo gelöscht, muss auch der DNS-Eintrag `auto` weg, sonst könnte ein Fremder
  die Adresse bei GitHub Pages für sich beanspruchen.

Einrichtung der Anbindung: README des Dashboards, Abschnitt Auto.
