# Big Data in Biological Sciences :: SLU Uppsala

http://astrocyte.com/COST-CHARME/COST-CHARME/Home.html

---------

# Intro, random notes

- Erik Bongcam-Rudloff.(SLUBI/SGBC, Swedish University of Agricultural Sciences, Uppsala, Sweden): Opening of the training school an Practicalities explained

- [SLU Uppsala](http://slu.se/)
- COST actions - short scientific stays (1 month), Identify action, apply, visit.
- Sweden - 90% forests
- ~~karta lanczowa prepaid~~
- SMSes in Amsterdam on 31 dec 
- jak dzieci uczą się słów. monitoring w domu. Object tacking. Data analysis. Blue ...
 - context + frequency

# Monday 13-17 Jim Dowling: Lecture and hands-on training on Hops Hadoop. 

- _More data trumps smarter algorithms_
- PBs of data

- [reference human genome](https://en.wikipedia.org/wiki/Reference_genome)
- it turned out we only have around 24,000 genes
- SNP small nucl polymorphisms
- https://en.wikipedia.org/wiki/Photic_sneeze_reflex
 - https://blog.23andme.com/health-traits/sneezing-on-summer-solstice/
 
- google high throughput: process 40TB data/4 secs ; sequencing: 100gb/30 hours...


- Data Parallel Programming
- SCALA -dobry język do programowania i przetwarzania big data: https://www.scala-lang.org/
- Sweden has terrible problem with data storage. You can calculate a lot, but where to store data/results?

- Map reduce
- spark uses memory instead of disk

## Genomics

- NGS pipeline
- BGZF Block Gzip File - kompresja gzipem bloków, a nie całego pliku
- BAM Files - The BAM Format is a binary format for storing sequence data. https://genome.sph.umich.edu/wiki/BAM

## SPARK

### PySPARK

- https://docs.databricks.com/spark/latest/dataframes-datasets/introduction-to-dataframes-python.html
- pandas - dataframes integration


# Tuesday 

## 9-10 Gioele La Manno (Karolinska Institute): Introduction to machine learning

### PCAs

- dimensionality: obraz 128x128 px => 16384 dimensions!
- PCA - obrót wg dwóch (n) najważniejszych osi (koń 3D -> 2D)
- T-SNE - algrytm. t-distributed stochastic neighbor embedding (t-SNE) is a machine learning algorithm for dimensionality reduction developed by Geoffrey Hinton and Laurens van der Maaten.[1] It is a nonlinear dimensionality reduction technique that is particularly well-suited for embedding high-dimensional data into a space of two or three dimensions, which can then be visualized in a scatter plot. Specifically, it models each high-dimensional object by a two- or three-dimensional point in such a way that similar objects are modeled by nearby points and dissimilar objects are modeled by distant points. https://en.wikipedia.org/wiki/T-distributed_stochastic_neighbor_embedding
- linear mapping allows returning to the orginal space! -- tj odtworzenie zjawiska na podstawie PCA - generative model!!! :warning: :bulb:
 - PCA - to tylko obrót. Inna sprawa to to, co się wyświetla...
 - https://pl.wikipedia.org/wiki/Analiza_g%C5%82%C3%B3wnych_sk%C5%82adowych
 - http://ordination.okstate.edu/PCA.htm
 - https://stats.stackexchange.com/questions/158552/what-is-the-horseshoe-effect-and-or-the-arch-effect-in-pca-correspondence
 
### Clustering

- unsupervised learning
- define distance

### Regression

- logistic regression

### Error of the model

- https://en.wikipedia.org/wiki/Overfitting

### Classification

- Linear models: N points can be separated in N-1 dimensiosn

## 10-12:30 Marco Capuccini (Uppsala University): Machine learning in Spark hands-on. This is a short introductory lecture and followed by a hands-on.

- https://docs.google.com/presentation/d/1fFjBjqdA2L4LgjzX_jMWLEDVYGFRUnuIHjmBZEisq-o/edit#slide=id.p

- **apache spark** - successor of hadoop
- allows interactive analysis with jupyter notebook or apache zeppelin https://zeppelin.apache.org/
- OpenStack is a free and open-source software platform for cloud computing, mostly deployed as an infrastructure-as-a-service (IaaS). https://en.wikipedia.org/wiki/OpenStack
- Docker: `sudo docker run -p 8080:8080 -d mcapuccini/mllib-exercises`


### SVM

- C - what training error do we allow
- Optimization methods: Limited-memory BFGS (L-BFGS)

## 13:30-16:00 Apurva Nandan (CSC  - IT Center for Science, Finland): Spark SQL.

- spark sql dataframes: like in python
- dataframes lpeszy performance niż rdd
- immutable - nie można ich modyfikować (tj w tym samym obiekcie)
- https://github.com/csc-training/spark-sql
- jupyter notebook attached
- similar to pandas :warnin: :bulb:
- easy to use (my opinion)
- analysis of a live data (Twitter hashtags)
- apple mac - 20 rodzajów adapterów do HDMI/VGA... #strange...

## 16-17:00 Dr Vaughan Wittorff (PetaGene): “PetaSuite: Reducing the size and cost of NGS data storage and transfer”. 


- bardzo duży spadek kosztu sekwencjonowania; relatywnie koszt magazyniwania danych rośnie!
- Extremely Fast Compression algorithm http://www.lz4.org


# Wednesday 20.9.2017 9-12 Witold Rudnicki (University of Warsaw): Identification of informative variables in highly-multidimensional data  (machine learning hands-on with expression data).

- dwa rozkłady - czy się różnią?
- t-test - ale jak jest dużo zmiennych w próbce, to ciężko
- Bonferoni correction (FWER) - https://en.wikipedia.org/wiki/Bonferroni_correction
- false discovery rate
- information enthropy https://en.wikipedia.org/wiki/Entropy_(information_theory)
- random forests - lot of trees, randomized, democratic decision; dla każdego drzewa ograniczona liczba zmiennych



## R Studio

- BioConductoR - biblioteka


# 13:00-16:00 Kim Kultima, Payam Emami, Stephanie Herman and Ola Spjuth (Uppsala University): Large-scale medical metabolomics. Two major projects dedicated to this: Caramba.clinic and Phenomenal.

- metabolmics; chromatografia + MS (HPLC/MS?)
- Docker!
- Pachyderm - workflow system based on containers: http://www.pachyderm.io/


//We pay solid SF-based salaries along with significant equity because at this stage in our company's life, the right person is worth anything. We also offer full health benefits, unlimited vacation, flexible work hours and all the usual startup perks. //

- bardzo ważne jest wersjonowanie danych! git? :warning:

