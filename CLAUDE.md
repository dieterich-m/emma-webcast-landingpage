# CLAUDE.md – emma-webcast-landingpage

## Projektstruktur

Statisches HTML-Projekt für www.ite-consult.de/emma/. Wird via Vercel deployed (automatisch bei Push auf `main`).

**Parallel dazu existiert** `ite-consult-landingpage` (Next.js, separates Repo) — beide Projekte müssen bei WebCast-Updates synchron gehalten werden.

## WebCast-Terminpflege

Bei jedem neuen NetPlans WebCast-Termin diese Dateien aktualisieren:

| Datei | Was ändern |
|---|---|
| `emma/index.html` | `window.NETPLANS_FORM_URL` + Hero-Card (Label, Datum, Titel, Details) |
| `emma/termine/index.html` | `window.NETPLANS_FORM_URL` + Schema.org Event (name, startDate, endDate, location url, description) + Termin-Block (Datum, h2-Titel, Tagline, Kurzbeschreibung) |

**Aktueller Termin (Stand 27.04.2026):**
- Datum: Mittwoch, 20.05.2026 · 10:00–11:00 Uhr
- Titel: NetPlans Webcast | EMMA live: So sparen Unternehmen Zeit mit smarter Automatisierung
- URL: https://www.netplans.de/veranstaltungen/emma-im-einsatz-20-05-26/
- Format: Online · kostenlos

## Vergangene Events

Abgelaufene Event-Seiten vollständig entfernen (Seite + Sitemap-Eintrag + alle Links). Nicht einfach stehen lassen — schadet dem SEO.
