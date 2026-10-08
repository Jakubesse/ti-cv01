# cv01: Príkazový riadok a prvá stránka

Teória a ukážky: <https://beata.stehlikova.website.tuke.sk/ti/02.html>

**Odovzdávaš:** `index.html`, `style.css`, `obrazok.jpg`, `historia.txt`, `o-mne.txt` v tomto repozitári (commit a push do konca cvičenia) a rovnaké súbory na sigme v `public_html/ti/cv01`.

**Úloha 2.1: Zadanie a SFTP.** Prijmi zadanie *cv01* v Classroom 50 a repozitár naklonuj do `~/web/ti/cv01` podľa návodu [04 Odovzdávanie](https://beata.stehlikova.website.tuke.sk/navody/04-odovzdavanie.html). Rozšírenie SFTP sa v Kubeflow po reštarte niekedy stratí. Vráti ho tento príkaz v termináli:

```bash
code-server --install-extension Natizyskunk.sftp
```

Potom `F1`, **Developer: Reload Window**. Nastavenie pripojenia na sigmu zostáva, netreba ho robiť znova.

**Úloha 2.2: Pieskovisko.** V termináli v Kubeflow si vytvor `~/pieskovisko` a v ňom len príkazmi, bez myši, štruktúru `projekt/css`, `projekt/img` a prázdne súbory `projekt/index.html` a `poznamky.txt`. Jeden súbor skopíruj, jeden premenuj a jeden zmaž. Po každom kroku to over cez `ls -la`.

**Úloha 2.3: Vi.** V pieskovisku vytvor vo vi súbor `o-mne.txt` s tromi riadkami: meno, téma tvojho semestrálneho projektu, jedna vec, ktorú si sa dnes naučil. Ulož a odíď. Otvor ho znova, zmaž riadok cez `dd`, vráť ho cez `u` a odíď bez uloženia cez `:q!`. Cez `cat` over, že súbor má stále tri riadky.

**Úloha 2.4: História.** Na konci práce v termináli ulož históriu do súboru: `history > ~/pieskovisko/historia.txt`.

**Úloha 2.5: Stránka cez AI.** Prompt nižšie vlož do AI, na koniec doplň tému svojho projektu. Výsledok ulož do `~/web/ti/cv01` ako `index.html` a `style.css`. Obrázok pretiahni myšou z počítača do priečinka `cv01` v Exploreri a premenuj ho na `obrazok.jpg`. Stránku si pozri cez Five Server a čo nesedí, nechaj AI opraviť. Prečítaj komentáre v kóde: každý prvok musíš vedieť vysvetliť.

```text
Vytvor mi jednoduchú webovú stránku v HTML5 v slovenčine (lang="sk", kódovanie UTF-8)
a k nej samostatný súbor style.css. Bez JavaScriptu a bez frameworkov (žiadny Bootstrap).

Stránka je jedna (index.html) a má obsahovať:
- hlavičku s nadpisom h1 a menu, ktoré odkazuje na sekcie na tej istej stránke
  pomocou kotiev (href="#..."),
- sekcie s nadpismi h2, aspoň dva odseky textu, zvýraznené slovo (strong, em),
- nečíslovaný a číslovaný zoznam,
- tabuľku s hlavičkou (thead) a aspoň 3 riadkami, s viditeľným ohraničením buniek,
- obrázok zo súboru obrazok.jpg v tom istom priečinku, s atribútom alt,
- odkaz na externú stránku, ktorý sa otvorí v novej karte,
- pätičku s mojím menom a rokom.

CSS nech je jednoduché a čitateľné: písmo, obmedzená šírka obsahu a centrovanie,
farba nadpisov, menu vedľa seba, ohraničenie tabuľky, obrázok nesmie pretiecť mimo stránku.

Do HTML aj CSS daj krátke komentáre po slovensky, ktoré vysvetlia, na čo slúži
každý prvok, aby som kódu rozumel.

Téma stránky: [DOPLŇ]
```

**Úloha 2.6: Odovzdanie.** Skopíruj do zadania súbory z pieskoviska: `cp ~/pieskovisko/historia.txt ~/pieskovisko/o-mne.txt ~/web/ti/cv01/`. Potom commit a push podľa návodu [04 Odovzdávanie](https://beata.stehlikova.website.tuke.sk/navody/04-odovzdavanie.html).

**Úloha 2.7: Kontrola na sigme.** Pripoj sa cez `ssh` na sigmu a skontroluj, že v `public_html/ti/cv01` sú tvoje súbory (Ukážka 3). Ak priečinok chýba, vytvor ho a vo VS Code klikni pravým tlačidlom na priečinok `cv01`, **SFTP: Upload Folder**. Nakoniec otvor v prehliadači `https://sigma.tuke.sk/student/meno.priezvisko/ti/cv01/`.

---

# cv01: The command line and your first page (English)

Theory and examples: <https://beata.stehlikova.website.tuke.sk/ti/02.html> (switch to EN at the top)

**You submit:** `index.html`, `style.css`, `obrazok.jpg`, `historia.txt`, `o-mne.txt` in this repository (commit and push by the end of the lab) and the same files on sigma in `public_html/ti/cv01`.

**Task 2.1: Assignment and SFTP.** Accept the assignment *cv01* in Classroom 50 and clone the repository into `~/web/ti/cv01` following guide [04 Submitting](https://beata.stehlikova.website.tuke.sk/navody/04-odovzdavanie.html). The SFTP extension sometimes disappears from Kubeflow after a restart. This command in the terminal brings it back:

```bash
code-server --install-extension Natizyskunk.sftp
```

Then `F1`, **Developer: Reload Window**. The connection settings for sigma stay, you do not have to set them up again.

**Task 2.2: Sandbox.** In the Kubeflow terminal create `~/pieskovisko` and inside it, using commands only and no mouse, the structure `projekt/css`, `projekt/img` and empty files `projekt/index.html` and `poznamky.txt`. Copy one file, rename one and delete one. Check each step with `ls -la`.

**Task 2.3: Vi.** In the sandbox create a file `o-mne.txt` in vi with three lines: your name, the topic of your semester project, one thing you learned today. Save and quit. Open it again, delete a line with `dd`, bring it back with `u` and quit without saving with `:q!`. Check with `cat` that the file still has three lines.

**Task 2.4: History.** At the end of your terminal work save the history into a file: `history > ~/pieskovisko/historia.txt`.

**Task 2.5: A page made with AI.** Paste the prompt below into an AI and fill in the topic of your project at the end. Save the result into `~/web/ti/cv01` as `index.html` and `style.css`. Drag an image from your computer into the `cv01` folder in Explorer and rename it to `obrazok.jpg`. View the page with Five Server and let the AI fix whatever is not right. Read the comments in the code: you must be able to explain every element.

```text
Create a simple web page in HTML5 (set the lang attribute to the page language,
UTF-8 encoding) and a separate style.css file. No JavaScript and no frameworks
(no Bootstrap).

It is a single page (index.html) and it contains:
- a header with an h1 heading and a menu linking to sections on the same page
  using anchors (href="#..."),
- sections with h2 headings, at least two paragraphs of text, an emphasised word
  (strong, em),
- an unordered and an ordered list,
- a table with a header (thead) and at least 3 rows, with visible cell borders,
- an image from the file obrazok.jpg in the same folder, with an alt attribute,
- a link to an external website that opens in a new tab,
- a footer with my name and the year.

Keep the CSS simple and readable: font, limited content width and centring,
heading colour, menu items side by side, table borders, the image must not
overflow the page.

Add short comments in English to both the HTML and the CSS explaining what every
element is for, so that I understand the code.

Page topic: [FILL IN]
```

**Task 2.6: Submitting.** Copy the sandbox files into the assignment: `cp ~/pieskovisko/historia.txt ~/pieskovisko/o-mne.txt ~/web/ti/cv01/`. Then commit and push following guide [04 Submitting](https://beata.stehlikova.website.tuke.sk/navody/04-odovzdavanie.html).

**Task 2.7: Check on sigma.** Connect to sigma with `ssh` and check that your files are in `public_html/ti/cv01` (Example 3). If the folder is missing, create it, then in VS Code right-click the `cv01` folder, **SFTP: Upload Folder**. Finally open `https://sigma.tuke.sk/student/name.surname/ti/cv01/` in the browser.
