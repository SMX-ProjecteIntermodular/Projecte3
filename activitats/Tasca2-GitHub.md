# Títol de l'activitat

## Presentació de l'activitat

En el Projecte 3 us incorporareu a EverPia com a tècnics en pràctiques i, en equip, preparareu una proposta de conscienciació sobre la seguretat dels comptes i la informació. Per deixar constància del procés i dels resultats, cada alumne crearà el seu propi repositori privat a GitHub, que farà servir per documentar les activitats del projecte i compartir-ne el seguiment amb el professorat.

En aquesta activitat aprendreu a crear el repositori a partir d'una plantilla, configurar-lo i treballar-hi des de Visual Studio Code. Practicareu com editar documents Markdown en local, registrar els canvis amb commits i sincronitzar-los amb GitHub. També provocareu i resoldreu un conflicte entre una versió local i una de remota. Són eines i pràctiques habituals en projectes informàtics, que us ajudaran a mantenir la feina ordenada i a explicar amb claredat què heu fet.

### Durada de l'activitat

La durada prevista de l'activitat és 2 hores a classe per desenvolupar l'activitat, més el temps que necessiteu per documentar la resta d'activitats al repositori.

### Objectius específics de l'activitat

- Ús de control de versions amb Git i GitHub.
- Generació de documentanció en format Markdown.

### Competències treballades

j) Elaborar documentació tècnica i administrativa del sistema, complint les normes i reglamentació del sector, per al seu manteniment i l’assistència al client.

m) Organitzar i desenvolupar el treball assignat mantenint unes relacions professionals adequades en l’entorn de treball.

### Resultats d'aprenentatge i criteris d'avaluació

1713.5. Transmet informació amb claredat, de manera ordenada i estructurada.

### Continguts

- Control de versions amb git.
- Sincronització de repositoris amb GitHub.
- Resolució de conflictes.
- Documentació de projectes via GitHub i Markdown.

### Capacitats clau treballades

- Autonomia
- Organització del treball
- Resolució de problemes
- Responsabilitat

### Semàfor ús de la IA

🟠 Aquesta activitat permet un ús parcial o restringit.

Permès per com a eina de suport en la millora de la redacció dels informes, cerca preliminar d'informació, estructuració d'idees o explicació de conceptes teòrics complexos.

**Condicions**: Cal processar, entendre i validar sempre els resultats rebuts. Està totalment prohibit copiar l'enunciat d'un exercici directament al xat de la IA i enganxar la resposta generada per al lliurament final sense treball propi ni anàlisi crítica.

## Enunciat de l'activitat

### Requisits previs

- Tenir el vostre compte de GitHub creat, configurat correctament i operatiu.
- Visual Code a l'ordinador de l'aula o el vostre portàtil amb la configuració de GitHub per permetre la sincronització amb el vostre compte de GitHub.
- Es recomana la següent extensió de Visual Code:
  - `markdownlint`: per comprovar la sintaxi Markdown mentre escriviu.

### Fase 1: Creació del repositori i primeres configuracions

1. El primer pas serà crear un repositori a GitHub a partir de la plantilla `projecte3_template`. Aquest repositori serà el que utilitzareu per documentar les activitats realitzades durant el projecte 3. És molt important que marqueu el projecte com **privat**.

2. Afegiu com a col·laboradors del repositori als professors de projecte. Els usuaris dels professors són els següents:

   - Carlos Alonso `carlesalonso`
   - Isabel Bosch `iboschmi`
   - Carles Fugarolas `cfugarolas`
   - Cristian González `CR1stiancom`

    A la guia 4 del material de suport trobareu les instruccions per realitzar aquestes dues accions.

3. Creeu una carpeta anomenada `projectes` dins del directori `Documents` i cloneu a dins el repositori creat anteriorment usant Visual Code.

4. Obriu el terminal de Visual Code i configureu el vostre nom d'usuari i correu electrònic amb les següents comandes:

   ```bash
   git config user.name "Nom i Cognoms"
   git config user.email *correu escola*
   ```
  
    ❗**Important**: El nom ha de ser el vostre **nom i cognoms reals**, per exemple "Joan Garcia Querol" i el correu electrònic ha de ser el vostre correu de l'escola.

5. Editeu l'arxiu `README.md` del repositori per incloure el vostre nom i cognoms iel del vostre company de grup. Un cop fet això, feu un commit, **recordeu que els commits han de ser descriptius** i sincronitzeu el repositori amb GitHub.

6. Comproveu a GitHub que el repositori s'ha actualitzat correctament.

### Fase 2: Documentació de l'activitat

1. A la carpeta `Tasca2` del vostre repositori creeu un fitxer anomenat `Tasca2-GitHub.md` on documentareu les activitats realitzades durant la sessió. **Tingeu en compte que el nom de l'arxiu ha de ser aquest exacte (respectant les majúscules i minúscules)**.

2. Crear una carpeta `img`dins de la carpeta `Tasca2` on guardareu les captures de pantalla que aneu fent durant l'activitat.

3. Afegiu com a títol principal `Tasca 2: GitHub` i com a seccions les diferents fases de l'activitat.

4. A la secció de la "Fase 1: Creació del repositori i primeres configuracions" documenteu amb explicacions i captures de pantalla la següent informació de la configuració (Settings) del vostre repositori:

   - A `General`, mostrar el nom del repositori.
   - A `Collaborators` mostrar que el repositori és privat i que heu afegit com a col·laboradors als professors indicats.
   > Els professors un cop reben la invitació com a col·laboradors, l'han d'acceptar per aparèixer com a col·laboradors del repositori, no patiu si en el moment de fer la captura apareixen únicament les invitacions pendents.

5. A la secció de la "Fase 2: Documentació de l'activitat" documenteu amb explicacions i captures de pantalla les següents accions:

   - Fer el commit corresponent a la realització del punt anterior i sincronitzar el repositori amb GitHub.
   - Mostrar a GitHub (captura de pantalla) que el fitxer `Tasca2-GitHub.md` s'ha creat correctament amb el format indicat dins de la carpeta `Tasca2` i conté documentat el contingut del punt 4 mostrant el text i les imatges corresponents.
   - Cliqueu sobre el botó `History` de l'arxiu a GitHub i mostreu amb una captura de pantalla l'historial de commits del fitxer `Tasca2-GitHub.md`. Indiqueu si la informació que es mostra és la correcta.

   Acabeu la fase fent un commit i sincronitzant el repositori amb GitHub.

### Fase 3: Resolució de conflictes

En aquesta fase, anem a provocar conflictes i veure com es poden resoldre. En aquest projecte veurem l'escenari més senzill, els conflictes els provoquem amb nosaltres mateixos, per no mantenir una bona sincronització entre el repositori local i el repositori remot de GitHub.

Per fer-ho, heu de seguir els següents passos:

1. Crea en el repositori local un fitxer anomenat `conflicte.txt` dins de la carpeta `Tasca2` i afegeix-hi el text següent:

   ```text
   Aquest és un fitxer de prova per provocar conflictes.
   ```

   Un cop fet, fes un commit i sincronitza el repositori amb GitHub.

2. Ara en **local** afegeix una segona línia al fitxer `conflicte.txt` amb el text següent:

   ```text
   Aquesta és la versió local del fitxer.
   ```

   Fes un commit, a la descripció indica clarament que l'edició s'ha fet des de local. **No el sincronitzis** amb el repositori amb GitHub.

3. Ara, des de GitHub, edita el fitxer `conflicte.txt` i afegeix una segona línia amb el text següent:

   ```text
    Aquesta és la versió remota del fitxer.
    ```

    Per guardar els canvis, fes clic a `Commit changes`. Escriu un missatge descriptiu per al commit on quedi clar que l'edició s'ha fet des de GitHub, deixa marcada l'opció `Commit directly to the main branch` i fes clic a `Commit changes`.

4. Observa com ara a Visual Code es mostra que hi ha un canvi per pujar i un canvi per baixar. Si passes el cursos per sobre sense clicar, veuràs que apareix un missatge indicant els commits que hi ha per pujar i per baixar.

5. Sincronitza el repositori amb GitHub. Com que hi ha un conflicte, apareixerà un missatge indicant que no es pot fer la sincronització i que cal resoldre el conflicte.

6. Resol el conflicte de manera que el fitxer `conflicte.txt` quedi amb el següent contingut:

   ```text
   Aquest és un fitxer de prova per provocar conflictes.
   Aquesta és la versió local del fitxer.
   Aquesta és la versió remota del fitxer.
   ```

  Hauràs de fer un commit de solució del conflicte i sincronitzar el repositori amb GitHub.

Documenta els diferents punts d'aquesta fase amb captures de pantalla i explicacions al fitxer `Tasca2-GitHub.md` dins la secció "Fase 3:Resolució de conflictes", fes un commit i sincronitza el repositori amb GitHub.

### Què cal lliurar, on i com?

Al final de la sessió heu de penjar el vostre repositori corresponent al projecte 3 a la tasca de Moodle `Tasca 2 - GitHub`. El repositori ha de cumplir els següents requisits:

- Haver-se creat a partir de la plantilla  `projecte3_template`.
- Ser privat.
- Haver afegit com a col·laboradors als professors de projecte.
- Tenir al `README.md` les dades corresponents al vostre nom i el del company de grup.
- Incloure a la carpeta `Tasca2` un fitxer `Tasca2-GitHub.md` amb la documentació de l'activitat realitzada.

**És obligatori** que l'edició es realitzi en local amb l'editor (Visual Code) i que es sincronitzi amb el vostre repositori de GitHub. No es permet l'edició directa al repositori de GitHub.

## Material de suport

- Material propi.[Guia 1. Iniciació a Git, GitHub i Visual Studio Code](https://github.com/SMX-ProjecteIntermodular/Guies/blob/main/git-github/01-iniciacio-git-github-vscode.md)

- Material propi. [Guia 2. Treballant en el repositori amb Git](https://github.com/SMX-ProjecteIntermodular/Guies/blob/main/git-github/02-comandes-git.md)

- Material propi. [Guia 3. Markdown per treballar amb repositoris](https://github.com/SMX-ProjecteIntermodular/Guies/blob/main/git-github/03-markdown.md)

- Material propi. [Guia 4. Creació de repositoris a partir de plantilla](https://github.com/SMX-ProjecteIntermodular/Guies/blob/main/git-github/04-crear-repositoris.md)

- Material propi. [Guia 5. Resolució de conflictes amb Git](https://github.com/SMX-ProjecteIntermodular/Guies/blob/main/git-github/05-resolucio-conflictes.md)

- GitHub. [Documentación de GitHub](https://docs.github.com/es)
