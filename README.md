-----------------------------------------------------------------------------
EasyCodeML 1.0 Readme -	Aug/15/2016

Fangluan Gao (raindy@fafu.edu.cn)
Chengjie Chen (ChengjieChen@stu.scau.edu.cn)

Copyright (C) 2016 Gao F. and Chen C.

Citation:

Gao F and Chen J, 2016. EasyCodeML: an interactive visual tool for CodeML analysis.


-----------------------------------------------------------------------------
1. INTRODUCTION
-----------------------------------------------------------------------------
EasyCodeML is an interactive visual tool for CodeML analysis. It provides two running modes, one for beginners (the preset mode, nested codon models with predefined parameters) and the other, for experienced users (the custom mode, independent codon models with user-defined parameters), respectively.

In the preset mode, evolutionary analysis can be carried out with just one click because all key parameters of the nested models, including the branch model (M0 vs. two ratio Model 2), the branch-site model (ModelA null vs. Model A), the site model (M0 vs.M3, M1a vs. M2a and M7 vs. M8) and the clade model (M2a_rel vs. CmC), were built in and CodeML analysis from data input to results output was pipelined.

Many experienced users need to create or modify the control files when using CodeML to meet different requirements. Therefore, the custom mode is implemented, in which all parameters for any single-model can be modified.

-----------------------------------------------------------------------------
2.	SYSTEM REQUIREMENT
-----------------------------------------------------------------------------

EasyCodeML requires a Java runtime environment (JRE). Before running this program, please make sure the correct installation of JRE 1.6 (or higher). 

-----------------------------------------------------------------------------
3.	DATA PREPARATION
-----------------------------------------------------------------------------
3.1 Sequence File
EasyCodeML fully supports PAML format (i.e., examples/example.nuc, Li et al, 2016), so PAML file does not require any modification. .

3.2 Tree File
Tree file must be in Newick format (i.e., examples/example.trees, Li et al, 2016). Note that taxon names with illegal characters (such as spaces, semicolons) are not allowed and the pairs of parentheses must be properly nested.

-----------------------------------------------------------------------------
4.	ACKNOWLEDGMENTS
-----------------------------------------------------------------------------
We thank Mrs. Zhenxi Chen (Tropical crops genetic resources institute, CATAS), Han Li (Southwest University), Lin Zhang (Nanjing Normal University) for constructive feedback in the development of the program.

-----------------------------------------------------------------------------
5.	REPORTING BUGS AND FEEDBACK
-----------------------------------------------------------------------------
If you encounter any problems with EasyCodeML, please let us know. We will be sure to promptly track down and fix any bugs that are reported. If it is possible, also attach the data which caused the problems.
EasyCodeML is an on-going project. For any suggestions of further features that you would like to see included in the next version, please let me know as well. 