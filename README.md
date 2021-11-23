Originalus uzduoties failai randami original/, o pataisyti - solution/


Įsisavinti Make sistemai pateiktos keturios užduotys. Dvi užduotys yra kataloge bad_makefile ir dar dvi kataloge no_makefile.

Kataloge bad_makefile esančių C kodo Makefile'us reikės pataisyti, kad atitiktų Make sistemos keliamus reikalavimus. Atliktas užduotis įkelti į github'ą ir atsiųsti nuorodas.

Kataloge no_makefile yra dar du katalogai. Viename yra laikoma programos kodas, o kitame bibliotekos kodas. Nei viename iš jų nėra Makefile'o C kodo kompiliaivimui. Jums reikės juos parašyti. Atlitkas užduotis sukelti į github'ą ir atsiųsti nuorodą.

Reikalavimai program katalogui:

    Sukurti Makefile programai 'calculator'
    Programa susideda iš trijų .c failų: 'main.c', 'maths.c', 'usage.c'. Pagrindinis failas yra 'main.c'
    Kiekvienam .c failui turi būti sukurtas .o failas
    Keisti programos kodo negalima

Reikalavimai library katalogui:

    Parašyti Makefile bibliotekai ir programai, kuri naudoja biblioteką
    Programą sudarys tik 'main.c' failas
    Biblioteka sudarys 'file_reader.c' ir 'file_reader.h' failai
    Failas 'example_text.txt' yra naudojamas programoje
    Pagal nutylėjimą Makefile turi sukompiliuoti ir programą ir biblioteką
    Makefile turi būti aprašytas atskiras target'as, lendžiantis sukompiliuoti biblioteką nepriklausomai nuo programos
    Makefile turi sukurti .o failus bibliotekai ir programai

Pagalba:

    Kadangi bibliotekos failas nebus laikomas standartinėje linker'io paieškos kataloge, pasileisti programą tokiu būdu - LD_LIBRARY_PATH=`pwd` ./myprog
    LD_LIBRARY_PATH yra specialus kintamasis nurodantis linker'iui, kur dar ieškoti bibliotekų be jau jam nurodytų standartinių katalogų.
