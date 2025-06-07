Baza na sieci, z możliwością wspólnej współpracy przy zmianach, jeśli ktoś nie do końca ogarnia githuba, to dosłownie 5 komend żeby robić pushe wystarczy

robisz git clone

git clone git@github.com:Reklik/dezinformatorsieciowy3.git

robisz swojego brancha (jakby swoją wersję bazy)

git branch 6969420 (obojętnie co, ja wpisuje swój numer indeksu)

potem przechodzisz na swoją wersję

git checkout 6969420

potem edytujesz co chcesz edytować, poprawiasz pytania itd, następnie dodajesz zmiany i  sprawdzasz czy się zapisały komendą:

git status

dodajesz zmiany

git add .

commitujesz (czyli wrzucasz swoją wersję z komentarzem)

git commit -m "zmiana w pytaniu 69 bo nie ma fotki"

wypychasz swojego brancha na GitHub

git push -u origin 6969420

idziesz na GitHub https://github.com/Reklik/dezinformatorsieciowy3
zobaczysz żółty banner "Compare & pull request" - klikasz w niego

tworzysz Pull Request (MR)
sprawdź czy base: main, compare: 6969420
dodaj tytuł typu "poprawka pytania 69"
dodaj opis co zmieniłeś
kliknij "Create pull request"

czekasz aż admin zatwierdzi i zmerguje Twoje zmiany

WAŻNE - po zmergowaniu synchronizujesz się z główną bazą (bo ktoś innny mógł coś poprawić):

git checkout main
git pull origin main

jak chcesz robić kolejne zmiany, tworzysz nowego brancha:
git checkout -b moje-kolejne-zmiany
(i powtarzasz kroki 4-11)

UWAGI:
NIE pushuj bezpośrednio do main (nie będzie działać - chroniona gałąź)
Zawsze rób nowego brancha dla nowych zmian
Przed rozpoczęciem pracy zawsze zrób: git checkout main && git pull
