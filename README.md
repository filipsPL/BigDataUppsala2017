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


- dimensionality: obraz 128x128 px => 16384 dimensions!
- PCA - obrót wg dwóch (n) najważniejszych osi (koń 3D -> 2D)
- T-SNE - algrytm. t-distributed stochastic neighbor embedding (t-SNE) is a machine learning algorithm for dimensionality reduction developed by Geoffrey Hinton and Laurens van der Maaten.[1] It is a nonlinear dimensionality reduction technique that is particularly well-suited for embedding high-dimensional data into a space of two or three dimensions, which can then be visualized in a scatter plot. Specifically, it models each high-dimensional object by a two- or three-dimensional point in such a way that similar objects are modeled by nearby points and dissimilar objects are modeled by distant points. https://en.wikipedia.org/wiki/T-distributed_stochastic_neighbor_embedding
- linear mapping allows returning to the orginal space! -- tj odtworzenie zjawiska na podstawie PCA - generative model!!! :warning: :bulb:


