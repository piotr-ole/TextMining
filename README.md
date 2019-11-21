### Instrukcja

1. Trzeba doinstalować dwa pakiety: wikipedia i Morfeusz
2. Wikipedia: 
    pip: https://pypi.org/project/wikipedia/
    conda: conda install -c conda-forge wikipedia
3. Morfeusz:
    a. Trzeba wejść na stronę: http://morfeusz.sgjp.pl/download/
    b. Pobrać: Binding dla Pythona (jajko Pythonowe) [odpowiednią wersje do waszego Pythona]
    c. Uruchomić swoje środowisko (ja robiłem na condzie, ale pewnie tak samo w venv)
    d. Wejść do katalogu z jajkiem
    e. Odpalić: easy_install <plik_egg>
4. Można cieszyć się życiem

Pliki:
    - zawody.txt : zawiera zawody, które kategoryzował ten ziomek na magisterce
    - podzawody/ : każdy plik zawiera podzawody dla każdego z zawodów. Np. w sportowcy.txt będą piłkarz, tenisista itd. (klepałem to ręcznie)

Co obecnie nie jest rozwiązane i może być problematyczne:
    1. Żeby otagować tekst dla osoby np. 'Marek Edelman' potrzebuję znać listę jego form: ['Marek Edelman', 'Marka Edelmana'] itp.
    Wydaje mi się, że to jest problematyczne, ale do obejścia w jakiś sposób, kiedy już będziemy mieli znalezione pozycje osób w zdaniu.
    Można będzie robić tak:
        a. Szukać tych samych osób w dokumencie ( te same to te, dla których np. zgadza się 5 pierwszych znaków )
        b. Puszczać imię i nazwisko do Morfeusza (żeby znalazł podstawową formę) [Tego nie wiem jak zrobić !Trudne!]
        c. Mamy pozycję i formę, to szukamy w Wikipedii zawodu
        d. Tagujemy (Pytanie: jak tagować jak dana osoba ma wiele klas?)