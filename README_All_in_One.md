1️⃣ Repo structure

/Biblia_v1.0.md
/Prompts/
    01_Main_Prompt.md
    02_Iteration_Prompt.md
    03_Internal_Audit_Prompt.md
    04_External_Audit_Prompt.md
/Artefacts/
/Audit/Internal/
/Audit/External/
/Logs/

2️⃣ Roles & shortcuts
Rola	Emoji	Funkcja
LLM	💻	Generacja artefaktów, iteracje wg promptów
Agent	🤖	Selekcja, audyt wewnętrzny
Kurator	🧑‍💼	Zatwierdzenie artefaktów, mutacja Biblii
Audyt zewnętrzny	🌐	Analiza niezależna, dodatkowe insighty
3️⃣ Workflow & Iteracje
💻 Generacja → 🤖 Selekcja → 🧑‍💼 Zatwierdzenie / Mutacja Biblii
          → Audyt wewnętrzny → 💻 Iteracja
          → 🌐 Audyt zewnętrzny → Mutacja Biblii
4️⃣ Prompt Flow
/Prompts/01_Main_Prompt.md        -> 💻 Generacja artefaktów
/Prompts/02_Iteration_Prompt.md   -> 💻 Iteracje wg feedbacku
/Prompts/03_Internal_Audit_Prompt.md -> 🤖 Audyt wewnętrzny
/Prompts/04_External_Audit_Prompt.md -> 🌐 Audyt zewnętrzny
5️⃣ Quick Start – pierwsza iteracja

Wgraj Biblia 1.0 i prompty do repo.

💻 Uruchom prompt główny, wygeneruj artefakt w /Artefacts/.

🤖 Agent: selekcja i raport audytu wewnętrznego.

🧑‍💼 Kurator: zatwierdzenie/odrzucenie, aktualizacja Biblii.

🌐 Audyt zewnętrzny: niezależna analiza i insighty.

Aktualizacja prompt iteracyjnego → kolejna iteracja.

6️⃣ Practical Tips

Transparentność: każdy commit, log i artefakt audytowalny.

Artefakt powiązany z iteracją, promptem i autorem.

Wielomodelowy projekt: wszystkie LLM znają aktualną wersję Biblii i promptu.

Mutacja Biblii po każdej iteracji, jeśli wyniki wskazują poprawki.

💡 Efekt:

Gotowy workflow LLM + człowiek.

Artefakty zgodne z Biblią.

Pełna audytowalność i dokumentacja iteracji.

Szybki start dla nowych członków lub agentów.

               /Biblia_v1.0.md
                       │
                       ▼
                  /Prompts/
 ┌───────────────┬───────────────┬───────────────┐
 │ 01_Main       │ 02_Iteration │ 03_Internal   │
 │ _Prompt.md    │ _Prompt.md    │ _Audit.md     │
 │ 💻 Generacja │ 💻 Iteracja   │ 🤖 Audyt      │
 └───────────────┴───────────────┴───────────────┘
                       │
                       ▼
                   /Artefacts/
                   💻 Wygenerowane artefakty
                       │
                       ▼
              ┌────────┴─────────┐
              │                  │
         🤖 /Audit/Internal/     🌐 /Audit/External/
         Raport agenta           Raport zewnętrzny
              │                  │
              ▼                  ▼
          🧑‍💼 Kurator: Mutacja Biblii, zatwierdzenie artefaktów
                       │
                       ▼
          🔄 Nowa iteracja LLM wg zaktualizowanej Biblii

🔹 Krótkie wyjaśnienie

Biblia – centralny punkt odniesienia dla wszystkich promptów i workflow.

Prompty – główny, iteracyjny i audytowy (wewnętrzny / zewnętrzny).

Artefacts – LLM generuje, agent selekcjonuje, kurator zatwierdza.

Audyt – wewnętrzny i zewnętrzny raport, wykrywanie dziur i insighty.

Kurator – aktualizuje Biblię i inicjuje kolejną iterację.

Iteracje – powtarzany cykl aż do osiągnięcia celu projektu.
