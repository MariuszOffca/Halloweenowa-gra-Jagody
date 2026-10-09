# Halloweenowa gra Jagody

Gra urodzinowa z 13 duszkami zbieranymi przez kody QR. Każdy duszek ma animację, awatar i opis. Album zapisuje się lokalnie w przeglądarce uczestnika.

Strona: https://jagoda-duszki-halloween.shepard81.chatgpt.site/

## Pliki
- `gra/index.html` - strona główna i album.
- `gra/style.css` - wygląd strony.
- `gra/game.js` - postacie, opisy, mechanika i zapisywanie kolekcji.
- `gra/assets/` - filmy oraz obrazy.
- `kody-qr/` - 14 kodów: strona główna oraz 13 duszków.

## Uruchomienie
W folderze `gra` wykonaj `python -m http.server 8000`. Otwórz http://localhost:8000/ . Tryb próbny: http://localhost:8000/?test=1 .

## Ponowne wykorzystanie
Zmień teksty w index.html i game.js oraz materiały w assets. Na nową imprezę zmień klucze localStorage w game.js, aby utworzyć osobne albumy. Hosting statyczny wymaga zawartości folderu gra. Po zmianie domeny wygeneruj nowe QR z adresami `?ghost=ID`. Identyfikatory są w game.js.

Repozytorium nie zawiera albumów uczestników ani danych logowania. Publikowanie strony i jej dostęp ustawia się osobno na hostingu.
