# Prompt engineering i metaprompts: aprendre a demanar bé a la IA

## Presentació de l'activitat

Les eines d'IA generativa (Gemini, Copilot, ChatGPT, Claude...) poden estalviar moltes hores de feina, però només si se'ls sap demanar bé les coses. Un encàrrec vague dona una resposta vaga; un encàrrec precís dona un esborrany útil.

Aquesta activitat **no va de continguts: va de mètode i d'eines**. L'objectiu és que aprenguis una manera sistemàtica de treballar amb una IA (com es construeix un prompt, com es millora, com es verifica el resultat) i que te l'emportis per a qualsevol assignatura, mòdul o feina futura. El tema sobre el qual demanaràs coses és secundari i el triaràs tu.

És una **pràctica individual i guiada pas a pas**. No cal entregar cap document redactat: el que entregaràs és **el teu xat sencer**, perquè el valor està en el procés (com has anat demanant, corregint i comprovant), no en la resposta final.

### Durada de l'activitat

La durada prevista de l'activitat és 2 hores a classe: 50 minuts de teoria i 70 minuts de pràctica guiada individual.

### Eina de treball

- Eina recomanada: **Gemini** amb el compte del centre (és la que tenim disponible i permet compartir l'enllaç del xat). També pots fer servir Copilot, ChatGPT o Claude si ja hi treballes, sempre que puguis entregar el xat complet.
- **Tota la Part 1 i la Part 2 han d'anar dins d'un únic xat.** No obris xats nous ni esborris missatges: els intents fallits també s'avaluen.
- Anomena el xat: *PE - Nom Cognom*.
- La Part 3 (autoavaluació) es fa en un **xat nou i separat**.

### Objectius específics de l'activitat

- Identificar els elements d'un prompt eficaç (rol, context, tasca, format, públic i restriccions) i detectar quins falten en un prompt fluix.
- Aplicar tècniques bàsiques de prompt engineering: control del format de sortida, exemples (*few-shot*), descomposició pas a pas i millora iterativa.
- Entendre què és un **metaprompt** i fer-ne servir per generar, avaluar i millorar prompts propis.
- Verificar de manera crítica els resultats de la IA i detectar invencions o errors.
- Construir una petita **biblioteca personal de prompts reutilitzables**.
- Autoavaluar el propi treball amb una rúbrica i justificar la valoració amb evidències.

### Competències treballades

j) Elaborar documentació tècnica i administrativa del sistema, complint les normes i reglamentació del sector, per al seu manteniment i l'assistència al client.

m) Organitzar i desenvolupar el treball assignat mantenint unes relacions professionals adequades en l'entorn de treball.

n) Mantenir un esperit constant d'innovació i actualització en l'àmbit del sector informàtic.

o) Utilitzar els mitjans de consulta disponibles, seleccionant-ne el més adequat en cada cas, per resoldre en temps raonable supòsits no coneguts i dubtes professionals.

r) Adaptar-se a diferents llocs de treball i noves situacions laborals originats per canvis tecnològics i organitzatius en els processos productius.

---

## Part 1. Pràctica guiada de prompt engineering

Abans de començar, **tria un tema de treball** qualsevol que domines mínimament (un videojoc, un esport, muntar un PC, cuina, un tràmit, un tema d'un altre mòdul...). El tema només és l'excusa per practicar el mètode.

A cada pas: escriu al xat el que se't demana, llegeix la resposta i escriu-hi tu mateix una observació curta. Aquestes observacions teves dins del xat són part de l'entrega.

### Pas 1. La línia base: un prompt dolent a propòsit

1. Escriu al xat un prompt deliberadament vague sobre el teu tema. Per exemple:

   > Fes-me un resum sobre xarxes.

2. Llegeix la resposta sense tocar res.
3. Escriu al xat un missatge teu que comenci per *OBSERVACIÓ 1:* i digui **tres defectes concrets** de la resposta (massa genèrica, longitud inadequada, públic equivocat, format inútil, dades dubtoses...).

Aquesta primera resposta és la teva **línia base**: al final compararàs amb ella.

### Pas 2. Anatomia d'un bon prompt

Un prompt eficaç acostuma a tenir sis peces. Les recordarem com a **RCTFPR**:

| Peça | Pregunta que respon | Exemple |
|---|---|---|
| **R**ol | Qui vols que sigui la IA? | Ets professor de tecnologia de 4t d'ESO. |
| **C**ontext | Quina és la situació? | Preparo una sessió de 15 minuts per a alumnes sense coneixements previs. |
| **T**asca | Què ha de fer exactament? | Explica què és una adreça IP i per què serveix. |
| **F**ormat | Com ho vols rebre? | En 5 punts, màxim 2 línies cada punt. |
| **P**úblic | Per a qui és? | Per a alumnes de 15 anys. |
| **R**estriccions | Què no pot fer? | Sense anglicismes, sense parlar de subxarxes, sense inventar dades. |

**El que has de fer:** reescriu el prompt del Pas 1 incloent-hi les sis peces i envia'l. Després escriu *OBSERVACIÓ 2:* amb dues diferències que notes respecte de la línia base.

### Pas 3. Controlar el format de sortida

La IA respon en el format que li demanes. Si no l'hi dius, se l'inventa.

**El que has de fer:** demana-li la **mateixa informació del Pas 2** en un format diferent i molt concret. Tria'n un:

> Torna-m'ho en una taula amb tres columnes: Concepte | Explicació en una frase | Error típic.

Després escriu *OBSERVACIÓ 3:* dient per a què et seria útil cada format (text seguit, llista, taula) en una feina real.

### Pas 4. Donar exemples (few-shot)

Si li ensenyes com vols les coses, ho imita. Això és *few-shot prompting*.

**El que has de fer:** envia un prompt que inclogui **dos exemples teus** del resultat que esperes i li demani que en generi tres més amb el mateix estil. Per exemple:

> Genera preguntes de repàs seguint exactament aquest estil:
> Exemple 1: Què passa si dos equips tenen la mateixa adreça IP? (resposta curta, 1 frase)
> Exemple 2: Per què un cable mal crimpat pot donar connexió intermitent? (resposta curta, 1 frase)
> Ara genera 3 preguntes més sobre el mateix tema, amb el mateix format i dificultat.

Escriu *OBSERVACIÓ 4:* dient si ha respectat l'estil dels exemples i en què se n'ha desviat.

### Pas 5. Demanar-ho pas a pas (descomposició)

Les tasques grans surten millor si les trosseges o si demanes que raoni abans de respondre.

**El que has de fer:** tria una tasca una mica complexa del teu tema (planificar, comparar, decidir) i demana-la **en dues fases**:

> Fase 1: abans de respondre, llista els criteris que faràs servir per comparar les opcions i espera la meva confirmació.

Quan contesti, revisa els criteris, corregeix-ne algun i només llavors demana-li la fase 2 (la comparació feta). Escriu *OBSERVACIÓ 5:* comparant aquest resultat amb el que hauries obtingut demanant-ho tot de cop.

### Pas 6. Millora iterativa

Un prompt gairebé mai surt bé al primer intent. El que distingeix un usuari expert és **com corregeix**.

**El que has de fer:** sobre l'última resposta, fes tres iteracions seguides, una per missatge, amb instruccions de correcció concretes (no val dir "fes-ho millor"):

1. Una iteració de **longitud o densitat**: "Redueix-ho a la meitat sense perdre cap idea clau."
2. Una iteració de **to o públic**: "Reescriu-ho per a algú que no ha vist mai un ordinador per dins."
3. Una iteració de **contingut**: "Afegeix un exemple real a cada punt i elimina el punt 3, que no aporta res."

Escriu *OBSERVACIÓ 6:* indicant quina de les tres iteracions ha millorat més el resultat i per què.

### Pas 7. Verificació crítica

La IA pot inventar-se dades amb molta seguretat. No entregues mai res sense comprovar-ho.

**El que has de fer:**

1. Demana-li: *Marca quines afirmacions de la teva última resposta són fets verificables i quines són opinions o estimacions. Indica el teu nivell de confiança en cada fet.*
2. Tria **un fet concret** i comprova'l tu, fora del xat, en una font fiable.
3. Escriu *OBSERVACIÓ 7:* amb el fet comprovat, la font i si era correcte, incorrecte o imprecís.

### Pas 8. La teva fitxa de prompt

**El que has de fer:** escriu al xat la versió final i neta del teu millor prompt, amb aquesta fitxa:

> **Nom del prompt:**
> **Per a què serveix:**
> **Prompt complet:** (amb RCTFPR)
> **Variables a canviar:** (el que substituiràs cada vegada, entre claudàtors)
> **Com saber si ha funcionat:** (dues condicions)

---

## Part 2. Metaprompts

Un **metaprompt** és un prompt que no et dona el resultat final, sinó que **treballa sobre els prompts**: te'n genera un, te'l critica o te'l millora. És la manera més ràpida de pujar de nivell: en comptes d'escriure prompts cada vegada millors a base d'intuïció, fas que la IA t'ajudi a dissenyar-los.

Continua **al mateix xat** que la Part 1.

### Pas 9. Metaprompt generador

**El que has de fer:** envia aquest metaprompt (adaptat al teu tema):

> Ets expert en prompt engineering. No resolguis la tasca encara.
> Vull un prompt per a [la teva tasca]. Construeix-me el prompt òptim: inclou-hi rol, context, tasca, format, públic i restriccions, i explica en una línia per què has triat cada element.

Compara el prompt que t'ha construït amb el teu del Pas 8 i escriu *OBSERVACIÓ 8:* amb dues coses que ell ha previst i tu no.

### Pas 10. Metaprompt avaluador

**El que has de fer:** enganxa-li el **prompt dolent del Pas 1** amb aquesta instrucció:

> Avalua aquest prompt del 0 al 10 segons claredat, context, especificitat de la tasca, format i restriccions. Per a cada criteri digues què falla i reescriu el prompt en una versió millorada. No executis el prompt.

Escriu *OBSERVACIÓ 9:* dient si estàs d'acord amb la seva puntuació i en què no.

### Pas 11. Metaprompt amb entrevista

El problema habitual és que nosaltres mateixos no sabem prou bé què volem. Es resol fent que la IA ens entrevisti.

**El que has de fer:**

> Ets expert en prompt engineering. Vull crear un prompt reutilitzable per a [la teva tasca], però no tinc clar el detall.
> Fes-me les preguntes que necessitis, d'una en una, fins que tinguis prou informació. Quan la tinguis, digues-m'ho i genera el prompt final.

Respon honestament totes les preguntes. Escriu *OBSERVACIÓ 10:* amb la pregunta que t'ha fet pensar més.

### Pas 12. La teva biblioteca personal de prompts

**El que has de fer:** per acabar la Part 2, escriu al xat **tres prompts reutilitzables** amb el format de fitxa del Pas 8. Han de ser prompts que de debò pensis fer servir més endavant (per estudiar, per resumir, per corregir textos, per preparar exàmens, per documentar feina tècnica...). Com a mínim un ha de ser un **metaprompt**.

---

## Part 3. Autoavaluació amb rúbrica (xat nou)

Aquesta part es fa en un **xat nou i separat** del de les parts 1 i 2. Anomena'l *AUTOAVALUACIÓ PE - Nom Cognom*.

La nota la poses **tu**: la IA només t'ajuda a mirar-te la feina amb criteri. Procediment:

1. Enganxa al xat nou la **rúbrica** d'aquesta activitat (la taula de sota).
2. Enganxa la teva feina: els prompts finals del Pas 8 i del Pas 12, i tres o quatre de les teves observacions.
3. Envia aquest prompt:

   > Ets avaluador exigent però just. Et dono una rúbrica i la meva feina d'una pràctica de prompt engineering.
   > Per a cada criteri: digues en quin nivell em situaries, cita l'evidència concreta de la meva feina que ho justifica i indica exactament què hauria de fer per pujar un nivell. No inflis la valoració. Si no hi ha evidència d'un criteri, digues-ho clarament.

4. Llegeix-ho de manera crítica. **No has d'acceptar-ho tal qual.**
5. Escriu al xat la teva **taula d'autoavaluació definitiva**, amb aquest format:

   > | Criteri | El meu nivell | Evidència (on es veu al meu xat) | Hi estic d'acord amb la IA? |
   >
   > **Nota global que em poso:** __ / 10
   > **Dues coses que he après sobre el mètode:**
   > **Una acció concreta de millora per a la pròxima vegada:**

Es valora la **coherència** entre la nota que et poses, les evidències que aportes i el que es veu al xat de les parts 1 i 2. Inflar-se la nota sense evidències baixa la qualificació d'aquest apartat; detectar bé les pròpies mancances la puja.

### Rúbrica d'autoavaluació

| Criteri | Pes | 1. Insuficient | 2. Suficient | 3. Notable | 4. Excel·lent |
|---|---|---|---|---|---|
| **C1. Elements del prompt (RCTFPR)** | 15% | Prompts vagues, sense rol ni context | Hi ha tasca i algun element més | Apareixen gairebé tots els elements i són pertinents | Els sis elements estan treballats i justificats; les restriccions són útils de debò |
| **C2. Tècniques aplicades** | 15% | No s'aprecien tècniques | S'aplica alguna tècnica de manera superficial | S'apliquen format, few-shot i pas a pas correctament | S'apliquen amb criteri i s'explica per què cada tècnica encaixa amb la tasca |
| **C3. Millora iterativa** | 15% | No hi ha iteracions o són del tipus "fes-ho millor" | Hi ha iteracions però poc concretes | Tres iteracions amb instruccions clares i efecte visible | Les iteracions mostren una estratègia: cada correcció ataca un problema identificat |
| **C4. Ús de metaprompts** | 15% | No s'han fet servir | S'ha copiat un metaprompt sense adaptar-lo | Els tres metaprompts s'han adaptat al propi cas | S'han adaptat i se'n compara el resultat amb el treball propi, amb conclusions |
| **C5. Verificació crítica** | 15% | S'accepta tot el que diu la IA | Es comenta que caldria comprovar-ho, però no es fa | Es comprova un fet amb font i es diu el resultat | Es detecta una imprecisió o invenció i s'explica com s'ha vist |
| **C6. Biblioteca de prompts** | 15% | No hi ha prompts reutilitzables | Prompts copiats, difícils de reutilitzar | Tres fitxes completes i reutilitzables | Fitxes amb variables, criteris d'èxit i utilitat clara més enllà de l'activitat |
| **C7. Qualitat de l'autoavaluació** | 10% | Taula buida o nota sense justificar | Nota justificada vagament | Nivells coherents amb evidències citades | Autoavaluació honesta i precisa, amb mancances detectades i una millora concreta |

Equivalència orientativa: 1 = 0-4 punts, 2 = 5-6 punts, 3 = 7-8 punts, 4 = 9-10 punts.

---

## Què s'entrega

1. **Enllaç del xat de les parts 1 i 2** (xat compartit, amb totes les observacions numerades de l'1 al 10).
2. **Enllaç del xat d'autoavaluació** (Part 3), amb la taula d'autoavaluació i la nota justificada.

Per compartir un xat de Gemini: obre el menú del xat i tria *Compartir* o *Compartir i exportar*, crea l'enllaç públic i comprova que s'obre abans d'entregar-lo.

### Llista de comprovació abans d'entregar

- [ ] El xat porta el meu nom.
- [ ] Hi ha els 12 passos i es veuen els prompts que he escrit jo.
- [ ] Hi ha les 10 observacions numerades, escrites per mi.
- [ ] Hi ha la fitxa del Pas 8 i les tres fitxes del Pas 12 (una és un metaprompt).
- [ ] Al Pas 7 hi ha un fet comprovat amb la font.
- [ ] El xat d'autoavaluació és un xat diferent i conté la rúbrica, la taula i la nota.
- [ ] Els dos enllaços s'obren correctament des d'una finestra privada.
