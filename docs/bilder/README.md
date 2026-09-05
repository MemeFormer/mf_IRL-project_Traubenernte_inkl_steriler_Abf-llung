# Bildablage

Bilder bitte **hier ablegen und committen** (nicht als GitHub-Kommentar-Upload),
damit sie Teil der Repo sind und dauerhaft verfügbar bleiben.

Namensschema:
```
kessel_01.jpg
presse_01.jpg
flaschen_muendung_01.jpg
```

Einbinden in Markdown mit relativem Pfad:
```markdown
![Schlachtkessel](bilder/kessel_01.jpg)
```

## Warum nicht die `user-attachments`-Links?
Die von GitHub beim Drag&Drop erzeugten Links zeigen auf einen S3-Speicher
(`github-production-user-asset-*.s3.amazonaws.com`). Der ist an ein Issue/PR
gebunden, nicht an die Repo — und für externe Werkzeuge nicht zugänglich.
Committete Bilder sind versioniert, offline verfügbar und überall lesbar.
