# Darstellungs-Check (360px)

Kleine statische Testseite zur Reproduktion eines Viewport-Checks (z. B. `window.innerWidth < 360`) für die Darstellungsanforderung des **Digitale Befehls**.
Praktisch zum Nachstellen auf Geräten wie dem Samsung xCover 5, wenn die Anwendung wegen zu kleiner Viewport-Breite blockiert.

https://basti189.github.io/Digitaler-Befehl---Darstellung/

## Projektkontext

Der **Digitale Befehl** ist ein Projekt der **Deutschen Bahn**.
Die hier bereitgestellte Testseite ist **kein Produktivbestandteil**, sondern
eine **technische Hilfs- und Nachweisseite** zur Analyse des Verhaltens
verschiedener Endgeräte und Browser (z. B. Samsung xCover 5).

## Inhalt

- **Anforderung**: Text aus dem Anforderungskatalog (unter der Überschrift „Anforderung“)
- **Test**: beschreibt die Prüfung per `window.innerWidth`
- **Quelle**: URL
- **Stand**: Datum
- **Messwerte**: `innerWidth`, `clientWidth`, `visualViewport.width`, `visualViewport.scale`, `devicePixelRatio`

## Lokal starten (VS Code)

1. VS Code Extension **Live Server** installieren (Ritwick Dey)
2. `index.html` öffnen
3. Rechtsklick → **Open with Live Server**

## Testen auf Android (z. B. xCover 5)

- PC/Laptop und Smartphone im selben WLAN
- GitHub Pages oder Live Server URL auf dem Smartphone öffnen
- **Chrome Zoom / Anzeigegröße prüfen**:
  - Wenn `window.innerWidth` z. B. **339** beträgt, triggert der 360px-Check.
  - Bei z. B. **90% Zoom** kann `innerWidth` z. B. auf **376** steigen.
