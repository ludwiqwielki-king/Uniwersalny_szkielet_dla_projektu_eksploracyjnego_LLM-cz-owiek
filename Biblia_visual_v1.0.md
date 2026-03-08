# Biblia projektu – Wersja 1.0 (wizualna)

**Nazwa projektu:** [TU WPISZ NAZWĘ PROJEKTU]  
**Wersja Biblii:** 1.0  
**Data utworzenia:** [YYYY-MM-DD]  
**Autor / Kurator:** [IMIĘ / ORGANIZACJA]  

---

## 1️⃣ Cel Biblii

Zapewnienie spójności, kontroli jakości i transparentności w projekcie eksploracyjnym realizowanym w modelu **LLM + człowiek**.  
Umożliwia iteracyjne uczenie się, audytowalność i rozwój projektu poprzez cykle generacji → selekcji → zatwierdzenia → mutacji zasad.

---

## 2️⃣ Role w projekcie

| Rola | Odpowiedzialność | Emoji / oznaczenie |
|------|----------------|------------------|
| **LLM / Agent generacyjny** | Eksploracja przestrzeni rozwiązań, generowanie wariantów artefaktów | 💻 |
| **Agent weryfikujący** | Automatyczna selekcja wariantów, sprawdzanie zgodności z regułami, przygotowanie raportów audytowalnych | 🤖 |
| **Kurator / człowiek** | Ostateczne zatwierdzenie artefaktów, kontrola kierunku projektu, aktualizacja Biblii | 🧑‍💼 |
| **Audyt zewnętrzny** | Niezależna ocena artefaktów, wykrywanie dziur lub braków w logice projektu, generowanie dodatkowych insightów | 🌐 |

---

## 3️⃣ Zasady pracy

- 💻 **LLM**: Eksploracja wariantów, generowanie artefaktów zgodnie z promptem i aktualną Biblią.  
- 🤖 **Agent**: Wstępna selekcja, zgodność, raporty audytowalne.  
- 🧑‍💼 **Kurator**: Zatwierdzenie artefaktów, kierunek zmian, mutacja Biblii.  
- 🌐 **Audyt zewnętrzny**: Analiza artefaktów z perspektywy „czystego” LLM, wykrywanie dziur i dodatkowych insightów.

---

## 4️⃣ Iteracyjny workflow (schemat wizualny)

```text id="h4v9lq"
[Pomysł / Koncepcja]
          │
          ▼
[Definicja zasad w Biblii projektu]
          │
          ▼
[Prompt / Specyfikacja zadania]
          │
          ▼
💻 [LLM: generacja wariantów artefaktów]
          │
          ▼
[Artefakt: obraz / tekst / kod / zadanie]
          │
          ▼
┌─────────▶🤖 [Agent: selekcja, zgodność, raport]─────────────┐
│         │                                                     │
│         ▼                                                     │
│   🧑‍💼 [Kurator: zatwierdzenie, korekta, kierunek zmian]      │
│         │                                                     │
│         ▼                                                     │
│   [Mutacja Biblii / wnioski]                                   │
│         │                                                     │
└─────────┴─────────┐                                           │
                    ▼                                           │
          💻 [Nowa iteracja LLM wg zaktualizowanej Biblii]      │
                    │                                           │
                    ▼                                           │
           🤖 [Audyt wewnętrzny: Git / Azure / Agent]           │
                    │                                           │
                    ▼                                           │
        💻 [Dalsza iteracja LLM wg wyników audytu]             │
                    │                                           │
                    ▼                                           │
           🌐 [Audyt zewnętrzny: LLM „czysty”]                 │
                    │                                           │
                    ▼                                           │
          [Aktualizacja Biblii wg audytów i wniosków]          │
                    └─────────────> powrót do 💻 LLM ───────────┘
          │
          ▼
[Efekt końcowy: stabilna wiedza + audytowalna dokumentacja]

/Biblia_v1.0.md        # Główna Biblia projektu
/Prompts/               # Prompt dla LLM
/Artefacts/             # Artefakty (obrazy, teksty, kod)
/Audit/Internal/        # Raporty audytu wewnętrznego 🤖
/Audit/External/        # Raporty audytu zewnętrznego 🌐
/Logs/                  # Logi działań LLM 💻 i człowieka 🧑‍💼

6️⃣ Wytyczne dla przyszłych projektów

Zachowaj pełną transparentność w repo.

Każdy agent LLM powinien mieć jasno określone uprawnienia i zakres działania.

Każdy artefakt musi być audytowalny, powiązany z iteracją, promptem i autorem.

Pętla 💻 → 🤖 → 🧑‍💼 → mutacja Biblii powinna być powtarzana aż do osiągnięcia celu projektu.

W razie wykrycia braków lub dziur – wprowadź audyt zewnętrzny 🌐.

💡 Praktyczna uwaga:
Ta Biblia 1.0 jest uniwersalna. Wystarczy dopisać specyfikę domeny projektu (komiks, grafika, narracja, analiza danych) i konkretne prompt + artefakty.
