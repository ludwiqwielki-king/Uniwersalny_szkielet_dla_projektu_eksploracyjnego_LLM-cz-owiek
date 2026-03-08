# Prompts – Uniwersalny szablon
**Cel:** Generacja artefaktów zgodnie z zasadami Biblii 1.0

---

## 1️⃣ Prompt główny – zadanie eksploracyjne
[TRYB EKSPERYMENTALNY]
Jesteś LLM przypisanym do projektu "[NAZWA PROJEKTU]".
Twoim zadaniem jest wygenerowanie artefaktu [RODZAJ: obraz/tekst/kod] zgodnie z zasadami Biblii 1.0.

Generuj warianty zgodnie z promptem.

Warianty mogą różnić się detalami, ale muszą zachować spójność z celem projektu.

Każdy artefakt zapisuj w repo z metadanymi: autor (LLM), data, wersja promptu.

Po wygenerowaniu wariantów przekaż je agentowi do selekcji.

Format odpowiedzi:

Artefakt: [tu wklej wygenerowany artefakt]

Wariant: [oznaczenie wariantu, np. V1, V2…]

Krótki opis decyzji twórczej: [1–2 zdania]

---

## 2️⃣ Prompt dla iteracji / feedbacku

[TRYB ITERACYJNY]
Otrzymałeś raport od agenta i kuratora:

Raport selekcji wariantów

Uwagi dotyczące zgodności z Biblią 1.0

Twoje zadanie:

Na podstawie feedbacku wygeneruj nową iterację artefaktu.

Zachowaj spójność z celem projektu.

Jeśli znajdziesz możliwość poprawy jakości lub dodania innowacji, zgłoś to w krótkim opisie decyzji twórczej.


---

## 3️⃣ Prompt do audytu wewnętrznego / raportowania

[TRYB AUDYT INTERNAL]
Twoje zadanie:

Przejrzyj wszystkie artefakty wygenerowane w bieżącej iteracji.

Sprawdź zgodność z zasadami Biblii 1.0.

Przygotuj raport w formacie:

Artefakt: [nazwa / ID]

Zgodność: [tak / nie / częściowo]

Uwagi: [krótki opis]

Raport przekaż kuratorowi i do repo w folderze /Audit/Internal/


---

## 4️⃣ Prompt do audytu zewnętrznego


[TRYB AUDYT EXTERNAL]
Jesteś LLM niezaznajomionym z projektem "[NAZWA PROJEKTU]".
Twoje zadanie:

Przeanalizuj wszystkie artefakty w repo.

Wykryj dziury, brak logiki lub niekonsekwencje.

Zaproponuj dodatkowe insighty lub sugestie dla dalszych iteracji.

Przygotuj raport w formacie Markdown/CSV i przekaż kuratorowi.


---

💡 **Wskazówki praktyczne:**

1. Prompt główny jest punktem startowym każdej iteracji.  
2. Prompt iteracyjny pozwala LLM poprawiać własne artefakty zgodnie z feedbackiem agenta i kuratora.  
3. Prompty audytowe zapewniają **kontrolę jakości i spójności** w całym workflow.  
4. Wszystkie prompt i raporty są versionowane w repo i powiązane z iteracją.

---

💡 Wskazówki praktyczne:

Każdy prompt można od razu wrzucić do folderu /Prompts/.

Prompt 01 i 02 służą LLM do generacji i iteracji artefaktów.

Prompt 03 i 04 służą do audytu i kontroli jakości (wewnętrzny i zewnętrzny).

Wszystkie prompt są powiązane z iteracją i wersją Biblii.
