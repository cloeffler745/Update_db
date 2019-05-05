<sub><u>Random viewing note:</u>
Sometimes the Jupyter notbook code will not render. When this happens paste the URL here:  [view Jupyter code](https://nbviewer.jupyter.org/)</sub>

# General Information

This repository is part of a larger database project that is working to merge multiple genomic reference databases.

The presented code maintains, updates, and edits a single database. The databases refered to here are not the actual reference databases holding genetic sequences. The database here is instead refering to a sql database where every row is associated with a single reference from the actual reference databases. These rows hold additional information about the respective reference genome. This includes information on:
* Strain, species, and genus universal taxanomic identifiers
* Strain, species, and genus scientific names
* The name of the reference database where the genetic information can be found
  * Current databases are:
    * [NCBI](https://www.ncbi.nlm.nih.gov/)
    * [Ensembl](http://fungi.ensembl.org/info/website/ftp/index.html)
    * [FungiDB](https://fungidb.org/common/downloads/release-41/)
    * [JGI 1000 Fungal Genomes Project](https://genome.jgi.doe.gov/fungi/fungi.info.html)
* Chromosome count
* Mean, minimum, and maximum chromosome lengths
* Contig counts
* Mean, minimum, and maximum contig lengths
* Mitochondrial DNA counts
* Mean, minimum, and maximum length of mitochondrial DNA
* Plasmid DNA count
* Mean, minimum, and maximum length of plasmid DNA


## Reference Database specific notes: 
### JGI 1000 Fungal Genomes Project

Updating the JGI part of the database is more complicated because JGI has many references have not been fully assembled and identified. Therefore, taxid information may change from update to update or species and genus level taxids may be missing all together. It is important to consider many possibilities that would not occur in other databases.
