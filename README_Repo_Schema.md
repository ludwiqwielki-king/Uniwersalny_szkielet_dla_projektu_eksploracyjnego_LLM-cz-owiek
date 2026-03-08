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
              ┌──────────┴───────────┐
              │                      │
          🤖 /Audit/Internal/       🌐 /Audit/External/
          Raport agenta             Raport zewnętrzny
              │                      │
              ▼                      ▼
          🧑‍💼 Kurator: Mutacja Biblii, zatwierdzenie artefaktów
                         │
                         ▼
              🔄 Nowa iteracja LLM wg zaktualizowanej Biblii

🔹 Wyjaśnienie przepływu

Biblia – punkt centralny, wszystkie prompty i workflow od niej zależą.

Prompty – główny prompt do generacji, prompt iteracyjny dla poprawek i prompt audytowy.

Artefacts – LLM generuje artefakty, które trafiają do audytu i kuratora.

Audyt – wewnętrzny (🤖) i zewnętrzny (🌐) raportuje niezgodności, wnioski i sugestie.

Kurator – ostateczne zatwierdzenie, mutacja Biblii i inicjacja kolejnej iteracji.
