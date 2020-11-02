# Comandos de la Práctica 01
## Azul Itania Rodriguez Ferrer

# Parte I. 

**Respuesta 1:**

/bin/bash 

**Respuesta 2:**

[mkdir] [opciones] [data/ filtered/ raw_data/ meta/ scripts/ figures/ archive/]

**Respuesta 3:**

[mv] [opciones] [filtered/ data/]
[mv] [opciones] [raw_data/ data/]

**Respuesta 4:**

Para organizar un proyecto bionformatico es necesario contar con un 
directorio  que a su vez se debe organizar en subdirectorios.
a) data/ : contiene los datos se le agrego dos subdirectorios (raw_data y 
filtered) esta organización es para que los datos crudos estén en 
un directorio (data/raw_data) y los modificados por análisis
subsecuentes en otros directorios (data/filtered). b) meta/ : se guardan los 
metadatos detallando la información de cada muestra. c) scripts/ :
en este directorio se guardan los scripts necesarios para correr el
análisis de principio a fin.d) figures/ : Se guarda el código que se utilice
sólo para hacer las figuras de la publicación.
e) archive/ : se usa para colocar scripts y datos que no se usan al 
momento pero puede ser de utilidad en un futuro, no se suben al repositorio. 

# Parte II.

**Respuesta 1:**
 
[ls] [-l] [delay.sh]

[chmod] [777] [delay.sh]

**Respuesta 2:**

[./] [] [delay.sh]

Después de la Parte I. necesito un descanso de exactamente 30 segundos.

**Respuesta 3:**

#!/bin/bash

echo "Después de la Parte I. necesito un descanso de exactamente 30 segundos."

sleep

echo "Ya puedo continuar!"

**Respuesta 4:**

ctrl + c

# Parte III
 
**Respuesta 1:**

[touch] [] [SarsCov-2.txt]

[nano] [] [SarsCov-2.txt]

[ls] [ -lth] [ SarsCov-2.txt]

[chmod] [777] [SarsCov-2.txt]

[./] [] [SarsCov-2.tx]

En la familia Corvidae se encuentras los alfa-coronavirus y beta-coronavirus 
SARS-coV2 que infectan principalmente a mamíferos; La estructura del genoma 
ya está estudiado lo que permite generar pruebas de PCR para su identificación  
así como las mutaciones que puedan presentarse en el. Durante la infección el 
dominio S1 se une a los receptores de la célula así como proteínas 
activadoras de la función de membranas. Conocer  la estructura molecular del
virus es importante para el desarrollo de vacunas o fármacos que bloqueen la 
unión del virus al receptor. Existen diversas estrategias de vacunas 
como usar virus atenuados o inactivados;una desventaja es que requiere de 
mucho tiempo y una inversión alta de dinero.

**Respuesta 2:**

[touch][][SarsCov-2_Spike.txt]

[nano][][SarsCov-2_Spike.txt]

[ls] [ -lth] [SarsCov-2_Spike.txt]

[chmod] [777] [SarsCov-2_Spike.txt]

[./] [] [SarsCov-2_Spike.txt]

Esta proteína se encarga se encarga mediar la union del coronavirus con la
célula huésped ya que contiene dos dominios (S1 y S2) que le van a permitir
unirse a receptores específicos. De igual forma, debe haber una transición
de la conformación de prefusión a posfusión
 
# Parte IV 
 
**Respuesta 1:**

[ln] [-s ~] [/filtered/splike_a.faa.txt]

[ls] [-s ~] [/filtered/splike_b.faa.txt]

[ls] [-s ~] [/filtered/splike_c.faa.txt]

**Respuesta 2**

[touch] [] [glycoproteins.faa.txt]

**Respuesta 3**

 [head] [] [splike_b.faa.txt]
>pdb|6VXX|B Chain B, SARS-CoV-2 spike glycoprotein

[head] [] [splike_a.faa.txt]
>pdb|6VXX|A Chain A, SARS-CoV-2 spike glycoprotein

[head] [] [splike_c.faa.txt]
>pdb|6VXX|C Chain C, SARS-CoV-2 spike glycoprotein

**Respuesta 4**

[less] []  [splike_*.faa.txt >> glycoproteins.faa]

**Respuesta 5**

[mv] [] [/Users/azulytania/GenomicaComputacional/arodriguez_p01/data/raw_data/spike_*.faa]

Las ligas simbólicas suaves creadas en data/filtered desaparecieron, dicho de otra forma, se
rompen 
 
**Respuesta 6**

[head] [-3]  [sarscov2_assembly.fasta.gz]

>NODE_1_length_264_cov_161.042781
CACAAATCTTAACACTCTTCCCTACACGACGCTCTTCCGATCTACGCCGGGCCATTCGTA
CGAACCGATACCTGTGGTAAAGGGTCCTACTGTATGGTGGTACACGAGTAGTAGCAAATG

[head] [-3] [sarscov2_genome.fasta]

>NC_045512.2 Severe acute respiratory syndrome coronavirus 2 isolate Wuhan-Hu-1, complete genome
ATTAAAGGTTTATACCTTCCCAGGTAACAAACCAACCAACTTTCGATCTCTTGTAGATCTGTTCTCTAAA
CGAACTTTAAAATCTGTGTGGCTGTCACTCGGCTGCATGCTTAGTGCACTCACGCAGTATAATTAATAAC

**Respuesta 7**

[grep]  [‘>’]  [sarscov2_assembly.fasta.gz | wc -l]
 *35*

[grep] [‘>’] [sarscov2_genome.fasta | wc -l]
 *1*
 
**Respuesta 8:**

[head] [-12]  [SRR10971381_R2.fastq]
@SRR10971381.512_2
CGTGGAGTATGGCTACATACTACTTATTTGATGAGTCTGGTGAGTTTAAAGTGGCTTCACATATGTATTGTTCTTTCTACCCTCCAGATGAGGATGAAGAAGAAGGTGATTGTGAAGAAGAAGAGTTTGAGCCATCAACTCAATATGAGT
+
/FFFA/A/FFFF66FFFFFF/FF/FFFFFFFFFFFFF/AFFF6FFFA6FFFFF/FFFFFFFFFFFFFFFFFF/FF/FFFFFA/FFF/FFF/A/AFA/FFFFF/=F/F/F/AFAFF//A/AFF//FFAF/FFF=FFAFFFA/A/6=///==
@SRR10971381.556_2
TTTGTAAAAATAAAATAAAAAAAATAAAAATAATATATTAAAAAAAGATAAATAAAAAAATGAACAATTAATAAAAAAAAAAAAAAAAAAAAATTAAAAAAAAAAAAAAAAAAAATAAAAAAAAAAAAAAATAAAAAAAAAATTATAAAA
+
6AFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF/FFFAFFFFFF/FFA/FF=F//=FF/FFFFFFFFFFFFFA/FFFF/FF/FA//F/FFFFFFA/=FFFFF/FFFF/F=FFFAFF///FFFFA/FF/6//////=/
@SRR10971381.1428_2
AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA
+
FFFFFFFFFFFFAFFFAFFFFFF6A//F//FFF


[grep] [‘@‘] [SRR10971381_R2.fastq | wc -l]
*130022*

**Respuesta 9**

El formato .fna hace referencia a secuencias de nucleótidos mientras que .faa a secuencias
de aminoácidos. Por otra parte .fastaq es un formato basado en texto para almacenar tanto una
secuencia biológica la linea con el @ es una forma de identificar la secuencia, la segunda linea
son letras de secuencia de nucleótidos sin procesar, en la tercer linea hay un  '+' y
opcionalmente va seguida de nuevo por el mismo identificador de secuencia (y cualquier
descripción), finalmente la línea 4 codifica los valores de calidad para la secuencia en la línea
2 y debe contener el mismo número de símbolos que letras en la secuencia. 

**Respuesta 10**

Con el comando less -S organiza la información en columnas y filas,  mientras que 
less muestra la información seguida. 

**Respuesta 11**

[cut]  [-f3] [ sarscov2_genome.gff3.txt | grep 'gene'| wc -l]
*11*
CDS es una region que pertence a un gene 

