# 🚀 AI Udviklingsopgaver 🤖

Velkommen til **AI Udviklingsopgaver**! Dette repository indeholder en samling af markdown-filer designet til at styrke din feature-udviklingsproces med AI-drevne IDE'er og kommandolinjeværktøjer. Oprindeligt bygget til Cursor [Cursor](https://cursor.sh/), fungerer disse værktøjer med enhver AI-kodeassistent, inklusive Claude Code, Windsurf og andre. Ved at bruge disse strukturerede prompts kan du systematisk arbejde dig gennem hele udviklingsforløbet – fra idé til implementering – med indbyggede kontrolpunkter til validering.

Stop med at kæmpe med store, uoverskuelige AI-forespørgsler – begynd i stedet at guide din AI-samarbejdspartner trin-for-trin!

## ✨ The Core Idea / Den Grundlæggende Idé

At bygge komplekse funktioner med AI kan nogle gange føles som en black box. Dette workflow har til formål at bringe struktur, klarhed og kontrol ind i processen ved at:

1. **Defining Scope / Definere Omfang**: Tydeligt beskrive, hvad der skal bygges, via et **Product Requirement Document** (PRD).

2. **Detailed Planning/ Detaljeret Planlægning**: Nedbryde PRD’en til en detaljeret, handlingsorienteret opgaveliste.

3. **Iterative Implementation/ Iterativ Implementering**: Guide AI’en til at løse én opgave ad gangen, så du kan gennemgå og godkende hver ændring.

Denne strukturerede tilgang hjælper med at holde AI’en på sporet, gør det nemmere at fejlfinde og skaber tillid til den genererede kode.


## Workflow: From Idea to Implemented Feature 💡➡️💻

Her er trin-for-trin-processen ved brug af .md-filerne i dette repository:

### 1️⃣ Create a Product Requirement Document (PRD)

Start med at lægge grundplanen for din funktion. Et PRD tydeliggør, hvad du bygger, for hvem og hvorfor.

Du kan oprette et letvægts-PRD direkte i dit foretrukne AI-værktøj:

1. Sørg for, at du har adgang til create-prd.md-filen fra dette repository.

2. I dit AI-værktøj, start PRD-oprettelsen:

    ```text
    Use @create-prd.md
    Here's the feature I want to build: [Describe your feature in detail]
    Reference these files to help you: [Optional: @file1.py @file2.ts]
    ```
    *(Pro Tip: For Cursor users, MAX mode is recommended for complex PRDs if your budget allows for more comprehensive generation.)*

    ![Example of initiating PRD creation](https://pbs.twimg.com/media/Go6DDlyX0AAS7JE?format=jpg&name=large)

### 2️⃣ Generate Your Task List from the PRD

Når dit PRD er færdigt (f.eks. MitFeature-PRD.md), er næste skridt at lave en detaljeret, trinvis implementeringsplan til din AI-udvikler.

1. Sørg for, at du har generate-tasks.md tilgængelig.

2. Brug PRD'et i dit AI-værktøj til at generere opgaver:

    ```text
    Now take @MyFeature-PRD.md and create tasks using @generate-tasks.md
    ```
    *(Bemærk: Udskift @MitFeature-PRD.md med det faktiske filnavn på det PRD, du lavede i trin 1.)*

    ![Example of generating tasks from PRD](https://pbs.twimg.com/media/Go6FITbWkAA-RCT?format=jpg&name=medium)

### 3️⃣ Examine Your Task List

Nu har du en velstruktureret opgaveliste, ofte med underopgaver, klar til AI’en. Det giver en tydelig køreplan for implementeringen.

![Example of a generated task list](https://pbs.twimg.com/media/Go6GNuOWsAEcSDm?format=jpg&name=medium)

### 4️⃣ Instruct the AI to Work Through Tasks (and Mark Completion)

For at sikre metodisk fremgang og give mulighed for validering, bruger vi process-task-list.md. Denne fil instruerer AI’en i at fokusere på én opgave ad gangen og vente på din godkendelse, før den går videre.

1. Sørg for, at process-task-list.md er tilgængelig.

2. I dit AI-værktøj, bed AI’en starte med første opgave (f.eks. 1.1):

    ```text
    Please start on task 1.1 and use @process-task-list.md
    ```
    *(Vigtigt: Du skal kun referere til @process-task-list.md for den første opgave. Instruktionerne i filen guider AI’en videre)*

    AI’en forsøger opgaven og beder dig derefter om at gennemgå resultatet.

    ![Example of starting on a task with process-task-list.md](https://pbs.twimg.com/media/Go6I41KWcAAAlHc?format=jpg&name=medium)

### 5️⃣ Review, Approve, and Progress ✅

Når AI’en fuldfører en opgave, gennemgår du ændringerne.

* Hvis ændringerne er tilfredsstillende, svar blot "yes" (eller en lignende bekræftelse) for at markere opgaven som fuldført og gå videre til næste.

* Hvis der er behov for rettelser, giver du feedback og beder AI’en rette opgaven, før der fortsættes.

Du vil se en tilfredsstillende liste over fuldførte punkter vokse, som giver et visuelt overblik over din funktions fremdrift!

![Example of a progressing task list with completed items](https://pbs.twimg.com/media/Go6KrXZWkAA_UuX?format=jpg&name=medium)

Selvom det ikke altid er perfekt, er denne metode en pålidelig måde at bygge større funktioner med AI-hjælp.

### 6️⃣ Video Demonstration 🎥

Hvis du vil se dette i aktion, demonstrerede jeg det på [Claire Vo's "How I AI" podcast](https://www.youtube.com/watch?v=fD4ktSkNCw4).

[![Demonstration of AI Dev Tasks on How I AI Podcast](https://img.youtube.com/vi/fD4ktSkNCw4/maxresdefault.jpg)](https://www.youtube.com/watch?v=fD4ktSkNCw4).

## 🗂️ Files in this Repository

* **`create-prd.md`**: Vejleder AI’en i at generere et Produktkravdokument (PRD) til din funktion.
* **`generate-tasks.md`**: Tager et PRD-markdown-dokument som input og hjælper AI’en med at nedbryde det i en detaljeret, trinvis implementeringsplan.
* **`process-task-list.md`**: Instruerer AI’en i at bearbejde den genererede opgaveliste én opgave ad gangen og vente på din godkendelse, før den går videre. (Filen indeholder også logik til at markere opgaver som fuldførte).


## 🌟 Benefits

* **Structured Development:** Sikrer en klar proces fra idé til kode.
* **Step-by-Step Verification:** Giver dig mulighed for at gennemgå og godkende AI-genereret kode trin for trin – for bedre kvalitet og kontrol.
* **Manages Complexity:** Bryder store funktioner op i små, overskuelige opgaver, så AI’en ikke farer vild eller genererer for kompleks eller forkert kode.
* **Improved Reliability:** En mere robust tilgang til at udnytte AI til større udviklingsopgaver, i stedet for ét stort prompt.
* **Clear Progress Tracking:** Visuel repræsentation af gennemførte opgaver gør det nemt at se, hvor langt du er, og hvad der mangler.

## 🛠️ How to Use

1. **Clone or Download:** Hent disse .md-filer ind i dit projekt eller et centralt sted, hvor dit AI-værktøj kan tilgå dem.

   git clone https://github.com/snarktank/ai-dev-tasks.git
   ```
3. **Follow the Workflow:** Brug .md-filerne systematisk sammen med dit AI-værktøj, som beskrevet i workflowet ovenfor.
4. **Adapt and Iterate:**
     * Du er velkommen til at ændre promptene i .md-filerne, så de bedre passer til dine behov eller din kodestil.
     * Hvis AI’en har problemer med en opgave, så prøv at omformulere funktionsbeskrivelsen eller nedbryd opgaverne yderligere.

## Tool-Specific Instructions

### Cursor

Cursor-brugere kan følge det beskrevne workflow ved at bruge .md-filerne direkte i Agent-chatten:

1. Sørg for, at du har adgang til filerne fra dette repository
2. I Cursor's Agent-chat, henvis til filer med @ (f.eks. @create-prd.md)
3. Følg det 5-trins workflow som beskrevet ovenfor
4. **MAX Mode til PRD’er**: Brug af MAX mode i Cursor ved PRD-oprettelse kan give mere grundige resultater, hvis dit budget tillader det


### Claude Code

Sådan bruger du værktøjerne med Claude Code:

1. **Copy files to your repo**: Kopiér de tre .md-filer til en undermappe i dit projekt (f.eks. /ai-dev-tasks)

2. **Reference in CLAUDE.md**: Tilføj disse linjer til din projekts ./CLAUDE.md-fil:
   ```
# AI Dev Tasks
Brug disse filer, når jeg beder om struktureret feature-udvikling med PRD’er:
/ai-dev-tasks/create-prd.md
/ai-dev-tasks/generate-tasks.md
/ai-dev-tasks/process-task-list.md

   ```

3. **Create custom commands** (optional): For nemmere adgang, opret disse filer i .claude/commands/:
   - `.claude/commands/create-prd.md` med følgende indhold:
     ```
     Brug venligst den strukturerede workflow i /ai-dev-tasks/create-prd.md til at hjælpe mig med at oprette et PRD for en ny funktion.
     ```
   - `.claude/commands/generate-tasks.md` med følgende indhold:
     ```
     Generér venligst opgaver ud fra PRD’et ved at bruge /ai-dev-tasks/generate-tasks.md  
Hvis der ikke er angivet et specifikt PRD, så generér en liste over tilgængelige PRD’er og bed brugeren vælge ét under `/tasks`, eller opret et nyt via `create-prd.md`:

- antag at PRD’er er gemt under `/tasks` og filnavnet starter med `[n]-prd-` (fx `0001-prd-[navn].md`)
- sørg for at filen ikke allerede har en tilsvarende opgaveliste i `/tasks` (fx `tasks-0001-prd-[navn].md`)
- **bed altid** brugeren bekræfte PRD-filnavnet før du fortsætter

Giv gerne valgmuligheder i nummererede lister, så jeg nemt kan svare.

     ```
   - `.claude/commands/process-task-list.md` med følgende indhold:
     ```
     Behandl venligst opgavelisten ved at bruge /ai-dev-tasks/process-task-list.md
     ```

   🔁 Sørg for at genstarte Claude Code efter at have tilføjet disse filer (/exit).
   Brug derefter kommandoer som /create-prd for hurtigt at starte workflowet.
  Bemærk: Denne opsætning kan også bruges globalt på tværs af alle dine projekter – se Claude Code-dokumentationen her
 og her.(https://docs.anthropic.com/en/docs/claude-code/memory) and [here](https://docs.anthropic.com/en/docs/claude-code/common-workflows#create-personal-slash-commands).

### Other Tools

For andre AI-drevne IDE’er eller CLI-værktøjer:

1. Kopiér .md-filerne til dit projekt
2. Referér til dem ifølge dit værktøjs dokumentation
3. Følg de samme workflow-principper

## 💡 Tips for Success

* **Be Specific:** Jo mere kontekst og klare instruktioner du giver (både i den oprindelige funktionsbeskrivelse og eventuelle afklaringer), desto bedre bliver AI’ens output.
* **Use a Capable Model:** Den gratis version af Cursor benytter i øjeblikket mindre kapable AI-modeller, som ofte har svært ved at følge de strukturerede instruktioner i dette workflow. For de bedste resultater, overvej at opgradere til Pro-planen for at sikre konsistent og præcis opgaveudførelse.
* **MAX Mode for PRDs:** Som nævnt tidligere, kan brugen af MAX mode i Cursor til PRD-oprettelse (create-prd.mdc) give mere grundige og højere kvalitetsresultater, hvis dit budget tillader det.
* **Correct File Tagging:** Sørg altid for at tagge PRD-filen korrekt (f.eks. @MitFeature-PRD.md) når du genererer opgaver.
* **Patience and Iteration:** AI er et kraftfuldt værktøj, men ikke magi. Vær forberedt på at vejlede, rette og iterere. Dette workflow er designet til at gøre iterationsprocessen nemmere.

## 🤝 Contributing

Got ideas to improve these `.md` files or have new ones that fit this workflow? Contributions are welcome!

Please feel free to:

* Open an issue to discuss changes or suggest new features.
* Submit a pull request with your enhancements.

---

Happy AI-assisted developing!
