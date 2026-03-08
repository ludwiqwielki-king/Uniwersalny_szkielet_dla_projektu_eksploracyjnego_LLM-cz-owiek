🔹 First Run Quick Reference – Nowy Projekt
🔹 Foldery w repo
/Biblia_v1.0.md
/Prompts/
/Artefacts/
/Audit/Internal/
/Audit/External/
/Logs/
🔹 Role i skróty

💻 LLM – generacja artefaktów zgodnie z promptem

🤖 Agent – selekcja, zgodność, raport wewnętrzny

🧑‍💼 Kurator – zatwierdzenie artefaktów, mutacja Biblii

🌐 Audyt zewnętrzny – niezależna analiza artefaktów

🔹 Workflow – skrót
💻 Generacja → 🤖 Selekcja → 🧑‍💼 Zatwierdzenie / Mutacja Biblii
          → Audyt wewnętrzny → 💻 Iteracja
          → 🌐 Audyt zewnętrzny → Mutacja Biblii
🔹 Pierwsza iteracja – kroki

Wgraj Biblia 1.0 i prompt główny do /Prompts/.

💻 Uruchom prompt główny, wygeneruj artefakt, zapisz w /Artefacts/.

🤖 Agent: sprawdzenie zgodności, przygotowanie raportu.

🧑‍💼 Kurator: zatwierdzenie / odrzucenie, aktualizacja Biblii.

🌐 Audyt zewnętrzny (opcjonalny) dla dodatkowych insightów.

🔹 Iteracje

Aktualizuj prompt iteracyjny i powtarzaj workflow aż do osiągnięcia celu projektu.

Każdy artefakt i raport zapisuj w repo z metadanymi.

Mutacja Biblii po każdej iteracji, jeśli wyniki wskazują na konieczne poprawki.

🔹 Wskazówki praktyczne

Zachowaj pełną transparentność – commituj każdą zmianę.

Każdy artefakt powinien być audytowalny i powiązany z iteracją, promptem i autorem.

Jeśli projekt jest wielomodelowy – upewnij się, że wszystkie LLM znają aktualną wersję Biblii i promptu.

💡 Gotowe – jedno miejsce do szybkiego startu, idealne jako cheat sheet dla zespołu lub agenta.
