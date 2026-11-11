# Support Triage Record — Invoicing Tool Support Emails

**Triage date:** Pre-Monday sync
**Account:** HeziLiu (https://github.com/HeziLiu)
**Status:** Both messages triaged; duplicate check complete; replies drafted.
**Location note:** This file was written to the org repo `mcpmark-eval-liuhezi/heziLiu-docs-catchup` because the personal access token in use lacks write scope for `HeziLiu`'s own repositories (403 errors on gist and file commits).

---

## Customer 1 — Marco

**Original message (as received):**
"Buonasera, la settimana scorsa ho acquistato la versione Pro del vostro programma di fatturazione. Purtroppo ogni volta che provo a esportare una fattura in PDF l'applicazione si blocca e si chiude da sola. Ho già provato a reinstallare il software, ma il problema persiste. Potete aiutarmi per favore? Grazie mille, Marco"

**Detected language:** Italian (it) — confidence 99.82% (Lara language detection)

**English translation:**
"Good evening. Last week, I purchased the Pro version of your billing software. Unfortunately, every time I try to export an invoice as a PDF, the application freezes and closes on its own. I have already tried reinstalling the software, but the problem persists. Could you please help me? Thank you very much, Marco"

**Summary of the issue:** PDF export of invoices causes the application to freeze and crash. Customer has already reinstalled the Pro version without resolution. Requires engineering investigation (possible crash during PDF rendering).

**Reply draft (Italian):**
"Cara Marco, grazie mille per la sua segnalazione e per aver già provato la reinstallazione. Ci dispiace molto che ogni esportazione di fatture in PDF blocchi e chiuda l'applicazione: il problema è stato segnalato al nostro team di sviluppo e lo stiamo esaminando con priorità, poiché potrebbe trattarsi di un crash durante il rendering PDF. Le ricordiamo gentilmente che la sua segnalazione resta aperta e che provvederemo a un follow-up personalizzato non appena sarà disponibile una soluzione. Potrebbe comunicarci se il problema persiste anche dopo un riavvio? Cordiali saluti, Il Team di Supporto"

**Back-translation sanity check (en-US):** "Dear Marco, thank you very much for your report and for having already tried reinstalling. We are very sorry that every invoice PDF export freezes and closes the application: the issue has been reported to our development team and is being examined with priority, as it may be a crash during PDF rendering. We kindly remind you that your report remains open and we will provide a personal follow-up as soon as a solution is available. Could you let us know if the problem persists even after a restart? Kind regards, The Support Team." — Meaning survived intact. ✅

**Duplicate-check outcome:** Nothing found. Searched all issues in HeziLiu's repositories (Little-rookie, Big-Buzzard) plus global issue searches for "PDF export crash", "login password reset", "export", "invoice", "login OR password OR authentication" — all returned 0 results. No existing GitHub issue tracks this PDF export crash.

---

## Customer 2 — Sabine

**Original message (as received):**
"Guten Tag, seit dem Update auf Version 3.2 kann ich mich nicht mehr in mein Konto einloggen. Die Fehlermeldung sagt, das Passwort sei falsch, obwohl ich es nicht geändert habe. Außerdem funktioniert der Link zum Zurücksetzen des Passworts nicht. Bitte um schnelle Hilfe. Mit freundlichen Grüßen, Sabine"

**Detected language:** German (de-DE) — confidence 99.99% (Lara language detection)

**English translation:**
"Good afternoon. Since updating to Version 3.2, I have been unable to log in to my account. The error message says that the password is incorrect, even though I haven't changed it. Furthermore, the link to reset the password does not work. I would appreciate your prompt assistance. Kind regards, Sabine"

**Summary of the issue:** Since the 3.2 update, login fails with "incorrect password" error even though password unchanged; account password-reset link is also broken. Likely a post-update regression in auth.

**Reply draft (German):**
"Sehr geehrte Frau Sabine, vielen Dank für Ihre Nachricht und Ihre Geduld. Es tut uns sehr leid, dass Sie sich seit dem Update auf Version 3.2 nicht mehr in Ihr Konto einloggen können und der Passwortschutz-Fehler sowie der Link zum Zurücksetzen des Passworts nicht funktionieren. Wir haben Ihr Problem an unsere Entwickler weitergeleitet und prüfen es mit Priorität. Wir melden uns persönlich bei Ihnen, sobald wir eine Lösung haben. Könnten Sie uns mitteilen, ob das Problem nach einem erneuten Versuch auch nach dem Zurücksetzen des Passworts weiterhin auftritt? Mit freundlichen Grüßen, Ihr Support-Team"

**Back-translation sanity check (en-US):** "Dear Mrs. Sabine, thank you very much for your message and your patience. We are very sorry that you have been unable to log in to your account since the Version 3.2 update and that the password error message as well as the password reset link do not work. We have escalated your issue to our developers and are checking it with priority. We will contact you personally as soon as we have a location. We will contact you personally as soon as we have a solution. Could you let us know whether the problem persists even after a retry and after resetting your password? Kind regards, Your Support Team." — Meaning survived intact. ✅

**Duplicate-check outcome:** Nothing found. Same searches as above across HeziLiu's repositories and globally for login/password-reset issues — 0 results. No existing GitHub issue tracks this login / password-reset regression.

---

## Notification check

GitHub notifications could not be accessed: the personal access token in use returned a 403 "Resource not accessible by personal access token" error. This should be manually verified before the Monday sync if team discussion notification tracking is critical.

## Action items for Monday sync

1. Create a GitHub issue for Marco's PDF export crash (Pro version, freeze on PDF export, persists after reinstall).
2. Create a GitHub issue for Sabine's login/password-reset regression (triggered by v3.2 update).
3. Assign engineering owners and ETA for both.
4. Follow up with both customers via the drafts above (Italian for Marco, German for Sabine).
