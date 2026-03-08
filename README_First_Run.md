🔹 First Run Guide – Nowy Projekt LLM + Człowiek
1️⃣ Przygotowanie repo

Utwórz strukturę repo zgodnie z Biblią 1.0:

/Biblia_v1.0.md
/Prompts/
/Artefacts/
/Audit/Internal/
/Audit/External/
/Logs/

Wgraj Biblia 1.0 i prompty do odpowiednich folderów.

Zaktualizuj pliki z nazwą projektu i datą.

2️⃣ Pierwsza iteracja generacyjna

Wybierz LLM do generacji (💻).

Uruchom prompt główny (01_Main_Prompt.md) dla pierwszego artefaktu.

Zapisz wygenerowane artefakty w /Artefacts/ z metadanymi:

autor

data

wersja promptu

wariant (V1, V2…)

Przekaż artefakty agentowi (🤖) do selekcji i wstępnej kontroli.

3️⃣ Kurator – zatwierdzenie i mutacja Biblii

Kurator (🧑‍💼) przegląda artefakty i raport agenta.

Zatwierdza lub odrzuca warianty, wskazując kierunek zmian.

Wprowadza ewentualne poprawki w Biblii projektu.

Każda zmiana wersjonowana w repo (commit + log).

4️⃣ Audyty
Audyt wewnętrzny (🤖)

Agent sprawdza zgodność artefaktów z Biblią.

Generuje raport i zapisuje w /Audit/Internal/.

Raport przegląda kurator i aktualizuje prompt/Biblię w razie potrzeby.

Audyt zewnętrzny (🌐)

LLM „czysty”, niezaznajomiony z projektem, analizuje artefakty.

Wykrywa dziury, niekonsekwencje i generuje dodatkowe insighty.

Raport zapisany w /Audit/External/.

Kurator integruje wnioski w Biblii i promptach.

5️⃣ Iteracje

Po audycie i zatwierdzeniu aktualizuj prompt iteracyjny (02_Iteration_Prompt.md).

Powtarzaj cykl:

💻 Generacja → 🤖 Selekcja → 🧑‍💼 Zatwierdzenie / Mutacja Biblii → Audyt wewnętrzny → 💻 Generacja → 🌐 Audyt zewnętrzny → Mutacja Biblii

Każda iteracja dodaje wartość, poprawia spójność i wzbogaca Biblię.

6️⃣ Dodatkowe wskazówki

Każdy artefakt, prompt i raport musi być audytowalny.

Zachowuj pełną transparentność w repo – każdy commit, komentarz i log są ważne.

Jeśli projekt jest wielomodelowy, upewnij się, że każdy LLM zna aktualną wersję Biblii i promptu przed generacją.

Po osiągnięciu celu projektu, przygotuj summary z wnioskami i dokumentacją iteracji.

💡 Efekt:
Po pierwszym uruchomieniu masz:

w pełni działający workflow generacyjny

artefakty zgodne z Biblią

audytowalną dokumentację i historię zmian

gotową Bazę Wiedzy dla kolejnych iteracji
