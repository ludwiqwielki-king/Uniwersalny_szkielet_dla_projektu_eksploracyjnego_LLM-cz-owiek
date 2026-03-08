🔹 Biblia 1.0 – Uniwersalny szkielet dla projektu eksploracyjnego LLM + człowiek
1️⃣ Informacje ogólne

Nazwa projektu: [TU WPISZ NAZWĘ]
Wersja Biblii: 1.0
Data utworzenia: [YYYY-MM-DD]
Autor / Kurator: [Imię / Organizacja]

Cel Biblii:
Zapewnienie spójności, kontroli jakości i transparentności w projekcie eksploracyjnym realizowanym w modelu LLM + człowiek.

2️⃣ Role w projekcie
Rola	Odpowiedzialność
LLM / Agent generacyjny	Eksploracja przestrzeni rozwiązań, generowanie wariantów artefaktów zgodnie z promptami i zasadami Biblii
Agent weryfikujący	Automatyczna selekcja wariantów, sprawdzanie zgodności z regułami, przygotowanie raportów w formacie audytowalnym
Kurator / człowiek	Ostateczne zatwierdzenie artefaktów, kontrola kierunku projektu, aktualizacja Biblii, decydowanie o iteracjach
Audyt zewnętrzny	Niezależna ocena artefaktów, wykrywanie dziur lub braków w logice projektu, generowanie dodatkowych insightów
3️⃣ Zasady pracy LLM i agentów

Zgodność z promptem: Wszystkie generacje muszą odpowiadać zadaniu określonemu w promptach.

Eksploracja wariantów: LLM może proponować różne warianty rozwiązania, w tym odchylenia od normy, pod warunkiem, że są raportowane agentowi.

Dokumentacja: Każdy artefakt musi być zapisany w repo z metadanymi: autor (LLM lub człowiek), data, wersja promptu.

Iteracja: Proces generacji → selekcji → zatwierdzenia → mutacji Biblii jest powtarzalny i audytowalny.

Kontrola jakości: Agent i kurator muszą każdorazowo weryfikować artefakty przed włączeniem ich do ostatecznej wersji projektu.

4️⃣ Zasady audytu

Audyt wewnętrzny: Sprawdzenie wszystkich commitów i artefaktów w repo pod kątem zgodności z Biblią.

Audyt zewnętrzny: Co jakiś czas LLM bez wiedzy o projekcie analizuje artefakty i raportuje potencjalne dziury, niekonsekwencje i dodatkowe wnioski.

Raporty: Wszystkie audyty muszą generować raport w formacie Markdown/CSV, który zostaje zapisany w repo.

5️⃣ Mutacja i rozwój Biblii

Aktualizacja zasad: Po każdej iteracji, kurator może wprowadzać zmiany w Biblii na podstawie wniosków z audytu lub obserwacji.

Historia zmian: Wszystkie zmiany w Biblii są versionowane w repo (commit + log).

Iteracyjna adaptacja: Biblię traktujemy jako żywy dokument, który ewoluuje wraz z projektem.

6️⃣ Struktura plików w repo
/Biblia_v1.0.md        # główna Biblia projektu
/Prompts/              # folder z promptami dla LLM
/Artefacts/            # wygenerowane artefakty (obrazy, teksty, kod)
/Audit/Internal/       # raporty audytu wewnętrznego
/Audit/External/       # raporty audytu zewnętrznego
/Logs/                 # logi działań agentów i człowieka
7️⃣ Wytyczne dla przyszłych projektów

Zachowaj pełną transparentność w repozytorium.

Każdy agent LLM powinien mieć jasno określone uprawnienia i zakres działania.

Każdy artefakt musi być audytowalny i powiązany z iteracją, promptem i autorem.

Pętla generacja → selekcja → zatwierdzenie → mutacja Biblii powinna być cykliczna aż do osiągnięcia celu projektu.

💡 Wskazówka praktyczna:
Ta uniwersalna Biblia 1.0 może służyć jako szablon dla dowolnego projektu, wystarczy dopisać specyfikę domeny (np. komiks, grafika, narracja, analiza danych) i zdefiniować prompt oraz artefakty.
