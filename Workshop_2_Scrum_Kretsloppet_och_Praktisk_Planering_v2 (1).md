# Workshop 2 – Scrum: Kretsloppet, Artefakter & Praktisk Planering

## 🎯 Översikt & Syfte
Denna workshop fokuserar på Scrums tre artefakter, deras tillhörande åtaganden (*Commitments*) samt de tidsboxade händelserna. Genom distansövningar får studenterna i sina ordinarie Boilerroom-grupper (2–5 personer) träna på att bryta ned produktmål till konkreta backlog-objekt, formulera sitt eget **Sprint Goal**, estimera arbete i grupp samt simulera de viktigaste Scrum-mötena.

---

## 📚 Del 1:  Artefakter, Åtaganden & Händelser

1. **De 3 Artefakterna & deras Åtaganden (Commitments)**
   * **Product Backlog** ➔ *Product Goal* (Långsiktigt mål som sätts av Produktägaren).
   * **Sprint Backlog** ➔ *Sprint Goal* (Mål för den aktuella sprinten, utformat och ägt av Scrum-teamet).
   * **Increment** ➔ *Definition of Done* (Kvalitetskravet för slutfört arbete).
2. **De 5 Tidsboxade Händelserna (Timeboxing)**
   * **The Sprint**: Behållaren för allt arbete (max 1 månad).
   * **Sprint Planning**: *Varför* är sprinten värdefull? *Vad* kan göras? *Hur* ska koden byggas?
   * **Daily Scrum**: 15 minuter dagligen av och för Utvecklarna för att parera mot Sprint Goal.
   * **Sprint Review**: Arbetsmöte med intressenter för besiktning av Incrementet och anpassning av backloggen.
   * **Sprint Retrospective**: Internt möte för kontinuerlig förbättring av arbetssätt och relationer.
3. **Det Agila Kretsloppet**
   * Hur mål, krav, daglig parering och kvalitetsstämplar samverkar i en iterativ snurra.

---

## 🛠️ Del 2: Distansövningar för Grupper 2–5 personer

### Övning 2A: Backlog Refinement, Sprint Goal & Estimering (40 min)
* **Verktyg:** Digital tavla (Miro / GitHub Projects / motsvarande) + Planning Poker-app (t.ex. *planningpoker.com* eller *pointingpoker.com*).
* **Viktig Scrum-princip:** Kursledaren/PO tillhandahåller endast **Product Goal** och användarberättelser (*User Stories*). **Teamet självt ansvarar för att formulera sitt eget Sprint Goal** under sin planering utifrån vad de väljer att ta sig an!

#### 🚜 Fiktivt Produktscenario: Fleet Management (Entreprenadmaskiner)
* **Använd den fork av[FleetManagmentrepo](https://github.com/Java-Fullstack-FJAX26/git-verkstad-pass-4) som ni jobbade med i förra veckan.
* **Product Goal (Från PO):** *"Skapa en central digital plattform för spårning av maskinparkens driftstatus, förebyggande underhåll och förarallokering med hög driftsäkerhet."*

#### 📋 Product Backlog (User Stories – Beskriver VAD, inte HUR):
1. **Statusspårning:** Som platschef vill jag kunna se realtidsstatus (`REDO`, `I_DRIFT`, `SERVICE_KRÄVS`) för alla entreprenadmaskiner samt kunna filtrera på maskintyper (t.ex. Grävmaskin, Vält, Hjullastare, Dumper), så att jag kan planera byggarbetsplatsens resurser.
2. **Förebyggande service & Larm:** Som verkstadsansvarig vill jag få ett automatiskt larm när en maskin passerar en drifttimmesgräns (t.ex. 200h) samt kunna boka in förebyggande service och sätta maskinens status till `UNDER_SERVICE`.
3. **Förarallokering & Behörighet:** Som projektledare vill jag kunna tilldela licensierade förare till specifika maskiner och få en varning om föraren saknar rätt körkortsklass (t.ex. C/CE eller traktorkort), så att vi uppfyller alla säkerhetskrav.
4. **Förbruknings & Kostnadsrapport:** Som ekonomiansvarig vill jag generera månatliga sammanställningar över körtid, bränsleförbrukning och tilläggskostnader per maskin och terrängtyp, så att vi kan fakturera rätt projekt.
5. **Akut Felanmälan & Ersättningsmaskin:** Som maskinförare vill jag kunna felanmäla en trasig maskin i fält via mobilen och omedelbart få förslag på närmaste tillgängliga ersättningsmaskin i samma kategoriklass.

---

#### 🔄 Arbetssteg för Övning 2A:

* **Steg 1 – Formulera teamets eget Sprint Goal & Task-nedbrytning (15 min):**
  * Gruppen granskar Product Backlog-objekten ovan.
  * **Formulera Sprint Goal:** Utvecklarna enas om och formulerar sitt eget **Sprint Goal** för den första sprinten baserat på de stories de bedömer är mest värdefulla att börja med.
  * **Bryt ned till Tasks:** Välj ut 2–3 User Stories och bryt ned dem till konkreta tekniska tasks (t.ex. domänklasser, databas/persistering, valideringsregler, gränssnitt och JUnit 5-tester).
* **Steg 2 – Planning Poker i Distansmiljö (25 min):**
  * Genomför en estimeringsrunda med Planning Poker (Story Points).
  * **Små grupper (2–3 personer):** Tillämpa *"Blind Show"* – båda/alla räknar till tre och visar sitt kort samtidigt så att ingen påverkar den andra i förväg.
  * Diskutera avvikelser (t.ex. en 2:a vs. en 8:a) och uppnå konsensus kring komplexitet, osäkerhet och risk.

---

### Övning 2B: Simulering av Daily Scrum & Retrospective (35 min)
* **Verktyg:** Breakout rooms med tidsmätare.
* **Uppgift:** Gruppen genomför två snabba rollspelsövningar i sina Boilerroom-grupper.

* **Moment 1 – Skarp Daily Scrum (15 min inkl. utvärdering):**
  * Genomför en strikt tidsboxad Daily Scrum på **exakt 5 minuter** (anpassad för en mini-sprint).
  * Varje medlem svarar kort med fokus på framsteg mot **sitt eget tillformulerade Sprint Goal** och eventuella hinder (*impediments*).
  * Utvärdera efteråt: Höll ni tidsboxen? Blev det ett statusmöte för en enskild person eller ett genuint avstämningsmöte för hela teamet?

* **Moment 2 – Mini-Retrospective med Sailorboat-mall (20 min):**
  * Använd en digital tavla med tre kolumner:
    1. **Vind (Vad hjälper oss framåt?):** Det som fungerade bra i samarbetet.
    2. **Ankare (Vad bromsar oss?):** Hinder, oklara krav eller teknisk skuld.
    3. **Förbättring (Vad gör vi annorlunda?):** Konkreta åtgärder.
  * Identifiera **1 konkret förbättringsåtgärd** som gruppen tar med sig direkt in i sitt nästa projekt.

---

## 📝 Redovisning & Inlämning
Gruppen dokumenterar sitt tillformulerade **Sprint Goal**, sin estimerade backlog med tasks samt sin förbättringsåtgärd från Retrospectiven i sin projektdokumentation.
