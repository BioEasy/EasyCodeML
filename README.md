**1.**      **Introduction**

EasyCodeML is an interactive visual tool for detecting selection in molecular evolutionary analysis. It implements the major codon-based models of CodeML in a simple and user-friendly interface.

EasyCodeML is written in Java. Precompiled versions are available for Microsoft Windows, Mac OS X, and Linux. We cannot guarantee that EasyCodeML will work well on other operating systems. The lastest version is 1.4.

**2.**      **Citing EasyCodeML**

The recommended citation for this program is:

Gao, F., Chen, C., Arab, D.A., Du, Z., He, Y., Ho, S.Y.W., 2019. EasyCodeML: A visual tool for analysis of selection using CodeML. Ecology and Evolution 9, 3891-3898.

**3.**      **System requirements**

Before running EasyCodeML, please ensure that your computer has a recent version of the Java Runtime Environment (JRE 1.6 or higher). The latest version of Java can be downloaded from http://www.java.com.

To export a tree as Newick format you will also need a recent version of FigTree (http://tree.bio.ed.ac.uk/software/figtree/).

**4.**      **Data preparation**

**4.1**  **Sequence alignment in PAML format**

CodeML requires a sequence alignment in PAML format. EasyCodeML includes a utility called Seqformat Convertor, which can automatically convert Clustal, FASTA, MEGA, Nexus, and Phylip formats into PAML format.

To convert sequence format in batch mode, type the following commands at the command prompt (CMD in windows or Terminal in Mac or Linux).

Parameter notes：

The parameters ‘-i’ and ‘-oF’ MUST be supplied and the parameters ‘-o’ and ‘-iF’ are optional.

java -cp EasyCodeML.jar SeqFormatConvert.seqFactory.SeqConverter -i -oF

-i		the directory to be read in

-o		the output directory

-iF		input sequence format

-oF		output sequence format [fasta (default)|MEGA|nexus|PAMLphylip]

Example:  

java -cp EasyCodeML.jar SeqFormatConvert.seqFactory.SeqConverter -i /Users/user1/Desktop -oF nexus

**4.2**  **Tree file** **in Newick format**

The tree file must be in plain Newick format (e.g., Examples/Example1.tree). The tree can not include branch lengths or bootstrap values and each node can have a single label. Taxon names should not have illegal characters (such as spaces and semicolons). 

 

**4.3**  **Labelling branches in the phylogenetic tree**

Tree labelling is necessary when using the branch-related models. To do this, press the ‘Label’ button in EasyCodeML, select the branch or clade to be treated as the foreground lineage, and press “done”.

​       In EasyCodeML, the symbols ‘#’ and ‘$’ are used for the branch or branch-site models and for the clade model, respectively. For the branch and clade models, if we have multiple foregroud branches (or clades) to be labelled (no more than 5), press the buttons 1st, 2nd, 3rd, 4th, and 5th to label each foregroud branch (or clade) in turn.  

**5.**      **Running the program** 

EasyCodeML provides two different running modes. The first is the preset mode, in which all key parameters of the nested models are built-in and which has pipelines for the selection analyses. The second running mode is the custom mode for experienced users. As with pamlX, the parameters for any codon-based model can be modified to meet different requirements.

The Quick Guide provides tutorials that illustrate the use of the two running modes. 

 

**6.**      **Tools menu in EasyCodeML**

| **Menu** | **Item**                | **Description**                                   |
| -------- | :---------------------- | ------------------------------------------------- |
| File     |                         |                                                   |
|          | Load Aligned   Sequence | Load a codon-based sequence   alignment           |
|          | Load Tree File          | Load a tree file in   Newick format               |
|          | Exit                    | Quit the program                                  |
| Tools    |                         |                                                   |
|          | LRTs   Calculator       | Retrieve *p*-values for LRTs                      |
|          | Control   File Editor   | Edit a CodeML   control file                      |
|          | Seqformat   Convertor   | Convert sequence alignment   to PAML format       |
|          | Tree Cleaner            | Convert tree file to NEWICK format                |
| Options  |                         |                                                   |
|          | Configure Tree   Label  | Modify tree layout   to fit in the display window |
| Help     |                         |                                                   |
|          | About                   | About EasyCodeML                                  |              
|          | User   guide            | Quick Guide for new   users                       |     
|          | Check for updates       | Update to the newest version                      |

 

**7.**      **Reporting bugs and feedback**

We welcome bug reports, feedback, and suggestions. For support please contact F. Gao (raindy[at]fafu.edu.cn) or C. Chen (ccj0410[at] gmail.com).

**8.**      **License**

Copyright 2018 by the EasyCodeML authors. EasyCodeML is freely available to non-commercial users and you are welcome to redistribute it under certain conditions. No guarantee of the functionality of this software, or of the accuracy of results obtained, is expressed or implied. Please inspect any results carefully. 
