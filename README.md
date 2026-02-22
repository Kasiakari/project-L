# ⚔ Karczma Pod Smokiem — D&D 5e Multiplayer

Przeglądarkowa gra RPG na zasadach D&D 5e z trybem multiplayer peer-to-peer.  
Zero rejestracji, zero serwerów — GM otwiera sesję, gracze dołączają kodem.

---

## 🚀 Jak zacząć

**Mistrz Gry:**
1. Otwórz stronę w przeglądarce
2. Wybierz **Mistrz Gry** → wpisz nick → kliknij **Utwórz sesję**
3. Dostaniesz **4-znakowy kod** (np. `K7M2`) — wyślij go graczom
4. Czekaj aż dołączą

**Gracze:**
1. Otwórz tę samą stronę w przeglądarce
2. Wybierz **Gracz** → wpisz nick → wpisz kod od GM → dołącz

> ⚠ GM musi mieć otwartą stronę przez całą sesję — pełni rolę serwera.

---

## 💬 Komendy czatu

Wpisz w pole wiadomości:

| Komenda | Efekt |
|---------|-------|
| `/roll k20` | Rzut kością 20 |
| `/roll 2k6` | Rzut dwoma kośćmi 6 |
| `/roll 2k6+3` | Rzut 2k6 z modyfikatorem +3 |
| `/roll k8-1` | Rzut k8 z modyfikatorem -1 |
| `/roll 4k4+5` | Dowolna kombinacja XkY+Z |

---

## 🎲 Panel Kości

| Przycisk | Efekt |
|----------|-------|
| k4 / k6 / k8 / k10 / k12 / k20 / k% | Rzut wybraną kością |
| **Przewaga** | Rzuca 2k20, bierze wyższy wynik |
| **Niekorzyść** | Rzuca 2k20, bierze niższy wynik |
| **Inne** | Wpisujesz własne wyrażenie np. `3k6+2` |
| Pole **Ilość** + **Modyfikator** | Ustaw przed kliknięciem kości |

Wszystkie rzuty są widoczne dla całej sesji w zakładce Czat.

---

## 📜 Karta Postaci

| Akcja | Efekt |
|-------|-------|
| Kliknięcie na cechę (SIŁ, ZRE...) | Rzut `k20 + modyfikator` widoczny dla wszystkich |
| Kliknięcie na umiejętność | Rzut `k20 + mod + biegłość` (jeśli zaznaczona) |
| Kropka przy umiejętności | Przełącza biegłość (dodaje premię do rzutów) |
| **Wyślij kartę do GM** | Wysyła całą kartę postaci do Mistrza Gry |

---

## 👑 Narzędzia GM

| Akcja | Efekt |
|-------|-------|
| **Karty graczy** | Podgląd kart postaci wszystkich graczy |
| **Tajny rzut GM** | Rzut k20 widoczny jako `GM 🔒` |
| **Zmień HP** | Kliknij kartę gracza → wpisz `-5`, `+3` lub nową wartość |
| **💾 Zapisz sesję** | Pobiera plik `.json` z kartami, inicjatywą i czatem |
| **📂 Wczytaj sesję** | Przywraca poprzednią sesję z pliku `.json` |

---

## ⚡ Inicjatywa

| Akcja | Efekt |
|-------|-------|
| **Auto-rzut** | Automatyczny rzut inicjatywy dla wszystkich (na podstawie ZRE) |
| Dodaj NPC / Potwora | Ręczne dodanie do kolejki z własną wartością |
| **→ Następna** | Przesuwa turę — widoczne dla wszystkich graczy |
| **Wyczyść** | Resetuje kolejkę inicjatywy |

---

## 💾 Zapisywanie sesji

GM może w każdej chwili zapisać sesję do pliku `.json` który zawiera:
- Karty postaci wszystkich graczy
- Kolejność inicjatywy
- Historię czatu
- Notatki GM

Aby wczytać sesję przy następnym spotkaniu: ekran startowy → **📂 Wczytaj zapisaną sesję** → wybierz plik → gra startuje automatycznie z nowym kodem.

---

## 🎭 Stany postaci

Każdy gracz może dodać sobie aktywny stan (widoczny lokalnie):  
`Oślepiony` · `Ogłuszony` · `Spętany` · `Przerażony` · `Zatruty` · `Niewidzialny` · `Leżący` · `Unieszkodliwiony` · `Nieprzytomny` · `Zauroczony`

---

## 📊 Skrócona tabela trudności (KS)

| KS | Poziom trudności |
|----|-----------------|
| 10 | Łatwe |
| 15 | Średnie |
| 20 | Trudne |
| 25 | Bardzo trudne |
| 30 | Niemal niemożliwe |

---

## ⚙ Technologia

- **PeerJS + WebRTC** — połączenia peer-to-peer bezpośrednio między przeglądarkami
- Zero serwerów, zero baz danych, zero rejestracji
- Jeden plik HTML — działa lokalnie lub hostowany np. na GitHub Pages
