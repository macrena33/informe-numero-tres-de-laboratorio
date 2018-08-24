# Laboratorio 03 - Ensamblaje de genomas y predicción de genes [![img](https://github.com/bioinf-biotec/labs_bioinf/raw/master/images/puzzle.png?raw=true)](https://github.com/bioinf-biotec/labs_bioinf/blob/master/images/puzzle.png?raw=true)



### Parte 1: El artículo genoma

------

**1.** ¿Cuántos *Sequencing Projects* y *Analysis Projects* hay depositados en GOLD? ¿Cuál es la diferencia entre ambos? [2]

- Sequencing Projects hay depositados 215.124 y en Analysis Projects hay depositados 174.491 , la diferencia es que el primero esta dirigido para la secuenciación y el segundo esta dirigido  al procesamiento informatico de un proyecto de secuenciacion.

  [Gold](https://gold.jgi.doe.gov/projects)

**2.** ¿Cuál es el dominio más representado en la base de datos, *archea*, *bacteria*, *eukaryote*, o *virus*? [1]

- El dominio mas representado es el de las bacteria.

  ![](https://github.com/macrena33/informe-numero-tres-de-laboratorio/blob/master/pregunta%20dos.2.png?raw=true) 

[Gold](https://gold.jgi.doe.gov/statistics)

**3.** ¿Cuáles son los *phyla* más representados entre los proyectos de genomas bacterianos en la base de datos? [1]

- La phyla mas representada en orden decreciente son proteobacteria, otras, firmicutes, actinobacteria.

  ![](https://github.com/macrena33/informe-numero-tres-de-laboratorio/blob/master/pregunta%20tres%20.3.png?raw=true)



[Gold](https://gold.jgi.doe.gov/statistics)

**4.** ¿A qué tipo de proyectos pertenece la mayor cantidad de genomas bacterianos depositados en GOLD? (tipo de proyecto, se refiere al tópico de la investigación, por ejemplo, salud humana, ambiental, etc.) [1]

- Pertenece a proyectos de tipo medico, seguido otros tipos de proyectos y por ultimo en la agricultura.

![](https://github.com/macrena33/informe-numero-tres-de-laboratorio/blob/master/pregunta%20cuatro.4.png?raw=true)

[Gold](https://gold.jgi.doe.gov/statistics)



**5.** ¿Cuál es el artículo original del genoma? (en el cual se reporta la sequenciación y ensamble del genoma) [2]

- El articulo original lleva por nombre The bonobo genome compared with the chimpanzee and human genomes y se encuentra en el siguiente link. https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3498939/

**6.** Explica, qué es el N50, L50, y NG50. [3]

- **N50** y **L50** son estadísticas de un conjunto de longitudes deconting o andamio . El *N50* es similar a una media o mediana de longitudes, pero tiene un mayor peso dado a los contigs más largos. L50 es el número de contigs cuya longitud sumada es *N50* .

- NG50, la **estadística NG50** es igual a *N50,* excepto que es el 50% del tamaño del genoma conocido o estimado que debe ser de la longitud NG50 o más. Esto permite comparaciones significativas entre diferentes conjuntos. En el caso típico en que el tamaño del conjunto no es más que el tamaño del genoma, la estadística NG50 no será más que la estadística N50.

   [Wikipedia](https://en.wikipedia.org/wiki/N50,_L50,_and_related_statistics)

**7.** ¿Cuál es el propósito de calcular estas estadísticas? [3]

- Se usa ampliamente en el ensamblaje del genoma especialmente en referencia a las longitudes del contigs dentro de un ensamblaje en borrador.

  [Wikipedia](https://en.wikipedia.org/wiki/N50,_L50,_and_related_statistics)

**8.** ¿Cuántos *contigs* conforman el genoma del Bonobo? ¿Cuál es el N50 y L50 del genoma? (responde basado en los *contigs*) [3]

- El genoma del Bonobo esta conformado por 121356 contigs, basados en la tabla L50 corresponde a 11048 y N50 a 66676.

  ![](https://github.com/macrena33/informe-numero-tres-de-laboratorio/blob/master/respuesta%208.2%20informe%203.png?raw=true)



**9.** ¿Cuál es el largo total y porcentaje de GC del genoma del Bonobo? ¿Qué quieren decir o qué indican éstos valores?

- El largo total es de 3286.64 (Mb) y el % de GC es de 42.3185. 

  [NCBI](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3498939/)

**10.** ¿Qué tipo de tecnología se uso para secuenciar el genoma del Bonobo? ¿Qué método (programa o algorítmo bioinformático) se usó para ensamblar el genoma?

- Segun el paper original de la secuenciacion del bonobo, se uso la plataforma illumina GaIIx2 y el sorfer de ensamblaje  Celera  assembler.

  [NCBI](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3498939/)

------

### Parte 2: Predicción de genes



**11.** Describe los resultados obtenidos. ¿Cuántos ORFs o genes encontró ORFfinder? ¿En qué hebra están codificados? ¿De qué largo son los ORFs predichos? ¿Algunos de ellos se sobreponen (fíjate en la posición de inicio [*start*] y término [*stop*])? [3]

- Segun lo reportado en NCBI se encontraron 7 ORFs en esta secuencia de los cuales 3 se encuentran en la hebra de 5' a 3' y los demas se encuentran de 3' a 5' y cuatro de ellos se detienen (ORF4 ORF5 ORF6 ORF7) y la longuitud de cada uno es: ORF1: 909|302, ORF4: 441|146, ORF5: 405|134, ORF7 144|47, ORF3: 99|32, ORF: 84|27, ORF2: 78|25.  

![](https://github.com/macrena33/informe-numero-tres-de-laboratorio/blob/master/WhatsApp%20Image%202018-08-23%20at%2017.54.44.jpeg?raw=true)

**12.** ¿Qué tipo de programa es ORFfinder, *Ab initio* o por homología? [2]

- Ab initio , estructura geneticacomo plantilla para detectar genes.

  

**13.** ¿A qué organismo pertenece la secuencia en cuestión? [2]

- Segun la herramienta BLAST el organismo corresponde a*Haemophilus Influenzae*  la cual es una bacteria.

  [BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi)

**14.** ¿Qué gen(s) está(n) codificados en la secuencia? [2]

- Son los ORF1 , ORF6 ORF7

  [NCBI](https://www.ncbi.nlm.nih.gov/orffinder/)

**15.** Tomando en cuenta la evidencia que acumulaste usando ORFfinder y BLAST. ¿Cuál o cuáles ORFs predichos por ORFfinder dirías tú que son o es el correcto(s)? [3]

- Segun ORFinder los ORF que codifican para proteinas son los mas correstos de los predichos, al ser insertados en la herramienta BLAST.

  [NCBI](https://www.ncbi.nlm.nih.gov/orffinder/) 

------

##### 