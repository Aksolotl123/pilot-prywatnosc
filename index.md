# Pilot — polityka prywatności

Obowiązuje od 30.10.2026.

Kontakt w sprawach prywatności: [tuz.lukasz@gmail.com](mailto:tuz.lukasz@gmail.com)

## W skrócie

- Pilot to aplikacja do automatyzacji telefonu (reguły: wyzwalacz → warunek → akcja). Działa na telefonie.
- **Autor aplikacji nie zbiera żadnych danych.** Pilot nie ma własnego serwera, kont użytkowników, reklam ani analityki.
- Reguły, dziennik zdarzeń i ustawienia są zapisane tylko w pamięci aplikacji na telefonie. Kopia reguł powstaje
  wyłącznie wtedy, gdy sam ją wyeksportujesz do wybranego pliku.
- Model językowy (Gemma) działa na telefonie — Twoje polecenia i opisy reguł nie są wysyłane do chmury.

## Usługa ułatwień dostępu

Pilot korzysta z usługi ułatwień dostępu Androida tylko do dwóch rzeczy:

- sprawdza, która aplikacja jest na wierzchu (wyłącznie jej nazwę), żeby Twoje reguły mogły reagować na otwarcie
  i zamknięcie aplikacji;
- naciska przyciski systemowe (ekran główny, wstecz, blokada ekranu, powiadomienia, ostatnie aplikacje, zrzut ekranu),
  gdy każe mu Twoja reguła albo Twoje polecenie.

Pilot **nie odczytuje zawartości ekranu ani wpisywanego tekstu**. Informacja o aplikacji na wierzchu nie opuszcza
telefonu. Przed użyciem usługi Pilot pokazuje to wyjaśnienie i prosi o zgodę; usługę możesz w każdej chwili wyłączyć
w Ustawieniach → Ułatwienia dostępu.

## Odczyt powiadomień

Jeśli na to zezwolisz, Pilot sprawdza tytuł i treść nowych powiadomień wyłącznie po to, żeby Twoje reguły mogły na nie
reagować (np. „gdy przyjdzie wiadomość ze słowem…”). Treść powiadomień nie jest nigdzie wysyłana ani zapisywana poza
dziennikiem zdarzeń na telefonie.

## Co i kiedy trafia poza telefon

| Kiedy | Co | Dokąd |
|---|---|---|
| Pobierasz model językowy w aplikacji | zwykłe żądanie pobrania pliku (Twój adres IP) | Hugging Face |
| Używasz modelu Gemma przez AICore | biblioteka Google ML Kit przesyła do Google anonimowe metryki użycia API (według dokumentacji Google — bez treści poleceń i odpowiedzi) | Google |
| Podasz adres i token Home Assistant | polecenia sterowania urządzeniami, które zaznaczysz, i lista urządzeń z Twojego serwera | **Twój** serwer Home Assistant / Dom Gemma |
| Dyktujesz polecenie mikrofonem | nagranie trafia do systemowego rozpoznawania mowy Androida | dostawca rozpoznawania mowy na telefonie (zwykle Google) |

Token Home Assistant jest przechowywany tylko w prywatnych ustawieniach aplikacji — nigdy w pliku reguł, eksporcie ani
dzienniku.

## Uprawnienia

Pilot prosi tylko o uprawnienia potrzebne do akcji i wyzwalaczy, których używasz (np. tryb Nie przeszkadzać, zmiana
ustawień systemowych, powiadomienia, pliki dźwiękowe do reguł z dźwiękiem, dostęp do sieci lokalnej dla Home
Assistant w domu). Każde możesz cofnąć w ustawieniach Androida.

## Usunięcie danych

Wszystkie dane Pilota usuniesz, odinstalowując aplikację albo czyszcząc jej dane w ustawieniach Androida. Autor nie ma
kopii Twoich danych.

## Wiek

Aplikacja jest przeznaczona dla osób pełnoletnich.

## Zmiany

O zmianach tej polityki informuje nowa data na górze strony.
