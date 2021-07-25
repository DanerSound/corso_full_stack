# CSS

CSS:

puoi' chiamare la roba css in tre modi diversi : 

- usando il tag link : ed il file si deve trovare nella stessa cartella in cui si trova il file html

    ```css
     <link rel="stylesheet" href="main.css"> 

    ```

- usando il tag diretamente in head :

    definendo delle cose qui vincoli il comportamento di tutti i tag h2, ce un discorso riguardo la precedenza/importanza 

    ```css
    <style type="text/css">
    	h2{
    		font-size: larger;
    		font-style: italic;
    		}
    </style>
    ```

- puoi definire il css direttamente inline :

```css
<h1 style="color: blueviolet;"> Questo è un titolo h1</h1>
<p style="background-color: chocolate;">Lorem ipsum dolor sit amet consectetur adipisicing elit. </p>
```

 

- i colori:  seguono la classe COLOR, possono essere scritti usano codice HEX, usano la notazione RGB  oppure RGBA ( alpha ) credo lo spazio fra i colori

- dato che il 90 percento delle volte si usa un file esterno: potrai sempre inserire, cosa per gestire i vari tag, ma anche il background, ci sono alcune definizioni che hanno bisogno di una sequenza ben precisa di tag per funzionare. ( vedi colori 2)

VEDI LEZIONE N3 E' LA PIU' IMPORTANTE

- per andare a modificare degli elementi in maniera piu' specifica ci sono i **selettori :**

    element ==> selezione per tipo di tag html;

    id;     ==> selezione per id;

    class;  ==> selezione per una intera classe di elementi;

    selezione per gerarchia : ovvero puoi fare riferimento a  piu' tag  contemporaneamente e quindi  essere piu' specifico per andare a modificare tag piu' interni 

    *; ==> seleziona tutti gli elementi della pagina;

SPECIFICITA' : date due dichiarazione contrastanti quale delle due vince ???

di base il colore di body viene ereditato dai tag interni 

ci sono 5 gradi di importanza : 

- 3  elemento ( tag)
- 2 classe (.nome)
- 1 #id
- priorita' 0 : corrisponde al codice CSS scritto INLINE

fonts : 

ricordati che devi usare in questo caso la  in primis il BODY che fa riferimento all'intero testo

per prendere qualcosa da google fonts : 

1-  PRENDERE IL LINK PRE COMPILATO

2- AGGIUNGERE LA FAMIGLIA DI OGGETTI NEL TAG BODY

Per modificare i paragrai singolarmente devi fare riferimoo alle classe o div 

em e' una unita di misura che vale 16px  e' usato molto spesso 

font-style : italic,

font-weight : bold

font-size : 130?%

Come allineare il testo al centro della pagina :

text-align : per potere alineare il testo in una certa posizione

text-decoration : pero potere aggiungere degli abbelimenti al testo

come personalizare lo speazi tra le verie righe ??

line-height : 80%  per avvicinare le righe oppure prendere piu' spazio 

BOX MODEL : 

per specificare il layout delle pagine HTML/CSS

si intende che ogni componente HTML puo' essere visto come un rettangolo avvolto da altri rettangoli :  NOTA BENE , data questo nuovo concetto tieni presente che i componenti si possono andare a prendere tutto la pagina riempiendo tutto il rettangolo.

quando modi

![CSS%20023abe741057485d9d15173da381bbf3/boxmodel1.jpg](CSS%20023abe741057485d9d15173da381bbf3/boxmodel1.jpg)

0- contenuto BLUE

1- padding SPAZIO BIANCO INTERNO TRASPARENTE

2- boder : a

3-margine  SPAZIO BIANCO ESTERNO TRASPARENTE

![CSS%20023abe741057485d9d15173da381bbf3/boxmodel2.jpg](CSS%20023abe741057485d9d15173da381bbf3/boxmodel2.jpg)

BOXMODEL 2 :

Box model e' esenziale per calcolare in maniera l'altezza e la lunghezza di un elemento

larghezza efettiva (width) : width + padding sx/dx+ border  sx/dx

alterzza effetiva (height) : height +padding up/down+ border  up/down

con l'utilizzo della proprieta' box-sizing possiamo fare in modo che anche i bordi e padding MA NON I MARGINI vengano inclusi nella definizione di alterzza e larghezza

```css
cosi lo puoi definire per tutti

* {
    box-sizing: border-box;
}

oppure puoi metterlo all'interno della dichiarazione del elemento
ATTENZIONE AGLI ELMENTI BLOCK LEVEL, HANNO BISOGNO DI ALCUNI 
MODIFICHE ANCHE ALL'INTERNO DEL CODICE HTML 

.elem {
 box-sizing: border-box;
}

```

FLEX BOX :

per potere ordinare piu' elemento di sulla pagina, e la semplificazione di  "inline element"

justify-content definisce come distribuire lo spazio tra gli elemento coinvolti nel FLAX-CONTAINER lungo gli assi principali. 

[https://developer.mozilla.org/en-US/docs/Web/CSS/justify-content?retiredLocale=it](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-content?retiredLocale=it)

align-items property:

Center the alignments for all the items of the flexible <div> element:

[https://www.w3schools.com/cssref/css3_pr_align-items.asp](https://www.w3schools.com/cssref/css3_pr_align-items.asp)


MEDIA QUERIES :

devi pensarala come del codice css specifico che viene chiamato in un particolare device
per potere fare le prove devi usare l'opzione smartphone the " inspection " 