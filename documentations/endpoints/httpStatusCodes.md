# All http status codes
## Successful
- `200`: **OK**	- Standard bei erfolgreicher GET/PUT/DELETE-Anfrage
- `201`: **Created** - Erfolgreiches POST, bei dem eine Ressource erstellt wurde
- `202`: **Accepted** -	Anfrage akzeptiert, aber noch nicht abgeschlossen (z. B. async Jobs)
- `204`: **No Content** -	Erfolgreich, aber ohne Rückgabedaten (z. B. DELETE ohne Body)

## Redirects
- `301`: **Moved Permanently** - API-Endpunkt dauerhaft verschoben
- `302`: **Found (Moved Temporarily)** -	Temporäre Umleitung (nicht REST-typisch)

❌ Client-Fehler (4xx)
Code	Bedeutung	Wann verwenden?
`400`: **Bad Request** - Ungültige oder fehlende Parameter
`401`: **Unauthorized** -Nicht authentifiziert (z. B. fehlendes Token)
`403`: **Forbidden**	- Authentifiziert, aber keine Berechtigung
`404`: **Not Found** -	Ressource nicht vorhanden
`405`: **Method Not Allowed** - HTTP-Methode nicht erlaubt (z. B. POST auf read-only Endpoint)
`409`: **Conflict** - Konflikt, z. B. Ressource existiert bereits
`422`: **Unprocessable Entity** - Validierungsfehler bei korrektem Request-Format

💥 Server-Fehler (5xx)
Code	Bedeutung	Wann verwenden?
`500`: **Internal Server Error** - Allgemeiner Serverfehler
`501`: **Not Implemented** - Funktionalität noch nicht verfügbar
`502`: **Bad Gateway	Fehlerhafte Antwort vom Upstream-Server
`503`: **Service Unavailable** - API (temporär) nicht verfügbar
`504`: **Gateway Timeout** - Timeout beim Upstream-Request
