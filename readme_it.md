# File di Informazioni Grafiche

È importante notare che questo standard grafico è molto nuovo ed embrionale. Le informazioni sono poche ma ben studiate.

## Cosa contiene l'archivio
Contiene sfondi e loghi che possono essere utilizzati nei software raster 2D tradizionali, che è il flusso di lavoro previsto (ad esempio, PhotoShop, Gimp, Paint3D).

La cartella è semplice ma pratica.

## Schema di colori
Il tema dei colori può essere rappresentato come un gradiente lineare tra colori come:
    magenta - ciano
    viola scuro - blu scuro

### NELL'IMPOSTAZIONE RGB, affinché il gradiente sia valido:
- Il blu deve essere bloccato a un numero N (0 - 255 / 0.0 - 1.0)
- Rosso + Verde devono essere uguali a N

> NOTA: evitare colori pastello, si intende dare un'atmosfera neon: palette di colori synthwave senza la grafica degli anni '80.

## Modello e Geometria
Sfruttiamo la modellazione 3D a basso poligono e le rifrazioni metalliche/vetrose, che sono diventate parte integrante del marchio.
Infatti, nessuna delle risorse fornite è stata realizzata con strumenti raster 2D.

Con "basso poligono" si intende modelli regolari con ombreggiatura piatta che celebrano la perfezione calcolata delle riflessioni, applicando shader raytraced metallici o simili al vetro (Beckmann o Multiscatter GGX), creando una struttura cristallina.

L'illuminazione è standard solo per un modello di cielo, che è descritto nell'esempio di flusso di lavoro.
> P.S. Usiamo Blender per quasi tutto e dei programmin in-house di contorno

## Esempio di flusso di lavoro
- Simulazione atmosferica raytraced (Nishita Sky) che ricorda lo spazio:
    - Ozono al massimo
    - O Polvere a 0.01, O Aria a 0.01

- Elementi di sfondo:
    - Qui si trova la libertà di programmazione, generazione procedurale, simulazioni fisiche o shader avanzati
    - Di solito un oggetto generato proceduralmente può essere stratificato (non composto) su un'immagine di sfondo

- PostProcessing:
    - HeavenParty non deve sovrasaturare o fare un uso intensivo di effetti raster, le mesh procedurali sono il suo punto di forza
    - Ma può essere applicato un nodo "glare" (impostazione Fog Glow, Threshold media, spread basso)

- Composizione:
    - Il logo può essere applicato DOPO o DURANTE il rendering (come oggetto nella scena o immagine stratificata)

> Ovviamente, il motore di rendering deve essere impostato su CYCLES

> Sono state fornite solo variazioni degli sfondi per semplicità, ma sentiti libero di richiedere altri asset più specifici in base al contesto.

> In seguito in questa cartella saranno forniti anche file .blend contenenti dati di esempio del marchio, nonché i lettori di file per eventuali software prioritari sviluppati dal personale interno di HeavenParty.

## Dettagli di LICENZA aggiuntivi:
Qualsiasi dei termini applicabili della licenza GNU AGPLV3 applicata al "Codice Sorgente" può essere applicata a questi asset.
Usa ma non abusare:
 - L'abuso include una o più delle seguenti azioni:
    - Rivendicare i file come propri
    - Utilizzare il marchio di HeavenParty senza autorizzazione

Grazie mille per la tua collaborazione.
Sylvio@HeavenParty