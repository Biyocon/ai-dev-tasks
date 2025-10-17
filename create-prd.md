# Rule: Generating a Product Requirements Document (PRD)

## Goal

At guide en AI-assistent i at oprette et detaljeret Produktkravdokument (PRD) i Markdown-format, baseret på en indledende prompt fra brugeren. PRD’et skal være klart, handlingsorienteret og egnet til, at en juniorudvikler kan forstå og implementere funktionen.

## Process

1.  **Receive Initial Prompt:** Brugeren giver en kort beskrivelse eller anmodning om en ny funktion eller funktionalitet.
2.  **Ask Clarifying Questions:** Før AI’en skriver PRD’et, skal den stille opklarende spørgsmål for at indsamle tilstrækkelig information. Målet er at forstå "hvad" og "hvorfor" funktionen skal udvikles – ikke nødvendigvis "hvordan" (det klarer udvikleren). Sørg for at stille spørgsmål med nummererede eller bogstaverede svarmuligheder, så brugeren nemt kan vælge.
3.  **Generate PRD:** Ud fra den oprindelige prompt og brugerens svar på de opklarende spørgsmål, skal AI’en generere et PRD med nedenstående struktur.
4.  **Save PRD:** Gem dokumentet som [n]-prd-[funktionsnavn].md i mappen /tasks. (n er et nulutfyldt 4-cifret tal startende fra 0001, fx 0001-prd-bruger-login.md, 0002-prd-dashboard.md osv.)

## Clarifying Questions (Examples)

AI’en skal tilpasse spørgsmålene efter konteksten, men her er typiske områder:

*   **Problem/Goal:** "Hvilket problem løser denne funktion for brugeren?" eller "Hvad er hovedmålet med denne funktion?"
*   **Target User:** "Hvem er den primære bruger af denne funktion?"
*   **Core Functionality:** "Hvilke nøglehandlinger skal brugeren kunne udføre?"
*   **User Stories:** "Kan du give et par brugerhistorier? (fx Som [brugertype], vil jeg [handling], så jeg kan [fordel].)"
*   **Acceptance Criteria:** "Hvordan ved vi, at funktionen er korrekt implementeret? Hvad er succeskriterierne?"
*   **Scope/Boundaries:** "Er der noget, funktionen ikke skal kunne?"
*   **Data Requirements:** "Hvilke data skal funktionen vise eller manipulere?"
*   **Design/UI:** "Findes der eksisterende mockups eller UI-guidelines?" eller "Hvordan skal funktionen se ud og føles?"
*   **Edge Cases:** "Er der nogen specielle situationer eller fejltilfælde, vi bør tage højde for?"

## PRD Structure

Det genererede PRD skal indeholde følgende afsnit:

1. **Introduktion/Overblik**: Kort beskrivelse af funktionen og problemet den løser. Beskriv målet.

2. **Mål**: Liste over specifikke, målbare mål for funktionen.

3. **Brugerhistorier**: Brugercentrerede scenarier, der beskriver hvordan funktionen anvendes og hvilken værdi den skaber.

4. **Funktionelle Krav**: Liste over specifikke funktioner, funktionen skal indeholde. Brug klar og præcis formulering (fx "Systemet skal tillade brugeren at uploade et profilbillede."). Nummerér kravene.

5. **Ikke-mål** (Uden for Omfang): Beskriv tydeligt, hvad denne funktion ikke skal inkludere for at afgrænse omfanget.

6. **Designovervejelser** (Valgfrit): Link til mockups, beskriv UI/UX, eller nævn relevante komponenter/stilarter hvis relevant.

7. **Tekniske Overvejelser** (Valgfrit): Nævn tekniske begrænsninger, afhængigheder eller forslag (fx "Skal integreres med eksisterende Auth-modul").

8. **Succeskriterier**: Hvordan måler vi, at funktionen er en succes? (fx "Øg brugerengagement med 10%", "Reducer support-henvendelser om X").

9. **Åbne Spørgsmål**: Liste over punkter, der stadig mangler afklaring.

## Target Audience

Antag at den primære læser af PRD’et er en juniorudvikler. Derfor skal kravene være eksplicitte, entydige og undgå teknisk jargon, hvor det er muligt. Sørg for, at der er nok detaljer til at forstå formålet og den grundlæggende logik i funktionen.

## Output

*   **Format:** Markdown (`.md`)
*   **Location:** `/tasks/`
*   **Filename:** `[n]-prd-[feature-name].md`

## Final instructions

1. Start ikke implementeringen af PRD’et
2. Stil altid opklarende spørgsmål først
3. Stil altid opklarende spørgsmål først
