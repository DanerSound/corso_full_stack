# boostrap

1- Intro:

quando usi BS, la classe " container " e' la classe piu' utilizzata e' tipo il semplice div o spam quando usi solo HTML.

( faccio riferimento agli esempi di base di BS 5 ufficiale ) 

si puo usare CDN ( content delivery network) : ovvero prendendo dei link messi a disposizione del portale, in questa modalita' quando fai riferimento a BS-5 devi aggiungere due link:

[https://getbootstrap.com/docs/5.0/getting-started/introduction/](https://getbootstrap.com/docs/5.0/getting-started/introduction/)

1- per la roba CSS :

- Da mettere dentro HEAD

2- per codice js ( per effetti tipo dropdown...!) : ce la possibilita di essere piu' selettivi e prendere singoli file, ma la versione humble ti permette di levarti il pensiero' subito.

- da mettere prima della fine  di BODY

si puo' usare in LOCALE: 

[https://getbootstrap.com/docs/5.0/getting-started/download/](https://getbootstrap.com/docs/5.0/getting-started/download/)

Devi cercare l'opzione da scaricare da qualche parte : e i file che servono solo sempre due ( il file zip contiene sicuramente tanti file)

bs: bootstrap.min.css

js: bootstrap.bundle.min.js

Vanno aggiunti nelle solite posizioni  di sopra: usando il tag link del html

quale e' meglio? 

entrambi sono approci validi, uno deve saperse decidere a seconda delle situazioni 

per avere una doppia sicurezza puoi lavorare usando CDN e avere cmq in file in locale per non fare mai riferimento. 

COMPONENTI FONDAMENTALI:  LEGGI IL CODICE HTML

CI SONO DEI CODICI DI PROVA PUI FARE LE PROVE INIZIALI CON QUELLE

[https://getbootstrap.com/docs/5.0/layout/containers/](https://getbootstrap.com/docs/5.0/layout/containers/)

- tre tipi di CONTAINERS generici:
    - container: CENTRA IL CONTENUTO ALL'INTERNO DELLA PAGINA
    - container fuild ESTENDE IL CONTENUTO PER TUTTA LA LUNGHEZZA DELLA PAGINA
    - container-{} si vedra' meglio nel sistema a grillia
    

BUTTONS:

devo fare sempre riferimento a btn, per aggiungere cambiare le caratteristiche devi aggiungere una classe in piu 

- 

badge: sono una sotto categoria diciamo permettono di implementare le notifiche, um numero crescente:

spaziattura : 

come aggiungere spaziatura in BS,  ricordati ce  il margine-m e padding-p 

guarda la documentazione : di spazio 

togli i Br e usa lo spazi :

aslcolta gli ulmiti minuti per fare degli esperimenti, Lo spazio tra i componenti lo devi mettere nella classe superiore che contiene l'emento interessato.

non mettere lo spazio direttamente nella classe del *compotente*  perche non funzionerebbe.

## Componenti Parte 2:

Componenti →  NAVBAR ( barra di navigazione!)

quando e' disposizione il COLLAPSE, QUESTO PERMETTE DI RENDERE LA BARRA DI NAVIGAZIONE RESPONSIVA RISPETTO IL DISPOSITIVO IN CUI VIENE VISUALIZZATO.

Molte note interessanti direttamente scrite sul codice HTML

dropdown: funziona con laggiunga del codice javascript, che contiene il pluging popper

NAV : per creare menu a forma di tabelle di navigazione

NOTA BENE LA DEFINIZIONE DELL-ID DELLE VARIE COMPONENTI, 

SE QUESTI NON CORRISPONDONO, LE TABELLE NON FUNZIONANO.

PILLS : 

ACCORDION:  E' un tipo di menu a tentina con si comprime  come un accordione

## Componenti Parte 3:

alcuni componenti sono formati da due pezzi, uno contienne una parte della chiave ( o id ) dell'altro 

per riuscire ad  attivare un particolare effeto.

nel caso del modal riguarda il data-bs-target="#staticBackdrop" : riguarda il pulsante che fara' l'azione .

<div class="modal fade" id="staticBackdrop" data-bs-backdrop="static"...> : ci interessa ID

se cambia l'ID , l'azione non si scatena piu'

per quanto riguarda i form, i vari moduli possono essere componibili con quello che vuoi, stai attendo alla classe e che li contiene e cosa contiene il container incui stai lavorando

Se metti qualcosa fuori del container questo non seguira le regole di BNS

## Componenti Parte 4:

Grid system :

e' il modo di organizzare i vari componendi 

row avvolte 12  unita' per forza basati si flexbox per layout responsivo

guarda bene l'esempio : di base prende la roba e la impila , puo' farle anche cambiare dimensione ma poco la spaziatura la prensenta la lezione dopo 

i breakpoint specificano una lunghezza appartire dalla quale non appena vai sotto quel punto BS compattera la riga. 

Quando ce solo un break poi impilla subito la roba. Quando hai piu breakpoi puoi fare cambiare la forma alla riga corrente

Allineamento : l'obbietivo di questa lezione e'  presentare la classe ORDER che  permette di arrangiare le collone in un ordine specifico. puoi usare delle soglie di guardia i break-point precendenti 

guarda gli esempio delle lezioni 5 e 6 sono piu' significativi