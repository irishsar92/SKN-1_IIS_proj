**Lifespan extension by daf-2 mediated IIS knockdown is dependent on interaction between transcription factor skn-1, temperature, and age  
**  
Sara D. Irish1, Annabel Kimberley1, Simone Immler1, Alexei A. Maklakov1  
		1School of Biological Sciences, University of East Anglia, Norwich Research Park, Norwich NR4 7TJ, UK  
		Corresponding author: S.irish@uea.ac.uk  
--------------------------------------------------------------------------------------------------------------------------------------  
Abstract:  
The highly evolutionarily conserved insulin signalling pathway (IIS) plays a critical role in the shaping of life-history traits through the regulation of downstream transcription factors, most notably daf-16, but also hsf-1 and skn-1. Reduced IIS (rIIS) has been shown to dramatically increase the lifespan of Caenorhabditis elegans nematodes. However, this work is typically performed in tightly controlled environments. Here, we used rIIS during development in skn-1 loss of function mutants under different constant and fluctuating temperature regimes. Our results indicate there is a critical period during development in which IIS, skn-1, and temperature interact to shape ageing trajectories.  

All datasets (described below) used can be found in the data folder, and all plots can be produced by running the chunks in the R markdown file titled: "plots.Rmd" and analysis in the file: "code.Rmd", both of which can be found in the code folder.   

---
File: SKN_N2_LS_15_25.csv  
Survival data for N2 and skn-1 mutants following daf-2 knockdown during development in 15 or 25°C. An additional treatment for skn-1 mutants involved developmental daf-2 knockdown with an additional cycle of the opposing temperature (15°C if they are otherwise housed at 25°C and vice versa) during the L2 stage of development.   
Columns:  
Block: experimental block ID number – only 1 block was included here  
Strain: N2 or SKN (skn-1 mutants) denotes the nematode strain  
Treatment: developmental treatments of daf-2 RNAi (daf) or controls (ev)  
Temperature: temperature nematodes are kept at: 15°C (15), 25°C (25), in addition to treatments with the developmental thermocycle – individuals kept at 15 with a 24-h stint in 25° (15F) or individuals kept at 25 with a 24-h stint in 15°C (25F)  
Plate.ID: plate ID number – nematodes were housed in plates of 10  
Worm: individual ID number nested within Plate.ID  
Death.Date: date of death  
Cause: cause of death (W = walling, M = matricide, E = exploded, D = natural death, L = lost due to human error)  
D1: start date of experiment  
Age: age (in days) at time of death  
Event: binary variables (1 = yes, 0 = no) for whether natural death occurred (this includes causes D and M)  
Exp: binary variable (1 = yes, 0 = no) for whether an individual exploded (this was included as rate of ‘explosions’ were high – death was counted as an explosion when an individuals cuticle burst)  
Inf:  binary variable (1 = yes, 0 = no) for whether a plate was infected during the assay  
  
---  
File: SKN-1_20C_LS.csv  
Survival data for skn-1 mutants following developmental daf-2 knockdown or controls (ev) when housed at 20°C.  
Columns:  
Block: experimental block ID number – only 1 block was included here  
Treatment: developmental treatments of daf-2 RNAi (daf) or controls (ev)  
Plate.ID: plate ID number – nematodes were housed in plates of 10  
Worm: individual ID number nested within Plate.ID  
Death.Date: date of death  
Cause: cause of death (W = walling, M = matricide, E = exploded, D = natural death, L = lost due to human error)  
D1: start date of experiment  
Age: age (in days) at time of death  
Event: binary variables (1 = yes, 0 = no) for whether natural death occurred (this includes causes D and M)  
Exp: binary variable (1 = yes, 0 = no) for whether an individual exploded (this was included as rate of ‘explosions’ were high – death was counted as an explosion when an individuals cuticle burst)  

---  
File: SKN1_20C_repro.csv  
Reproduction data for skn-1 mutants following developmental daf-2 knockdown or controls (ev) when housed at 20°C.  
Columns:  
ID: individual ID number  
Strain: only skn-1 mutants (SKN-1) were used in this assay  
Maturation Time: time at which individuals reached sexual maturity  
Treatment:  developmental treatments of daf-2 RNAi (daf) or controls (ev)  
D1-D5: number of offspring produced on given day of adulthood (Days 1 – 5)  

---  
File: Thermo_C_LS.csv  
Survival data for N2 and skn-1 mutant nematodes following developmental treatments with daf-2 RNAi or control treatment (ev). A rapid thermocycle was an additional treatment for all individuals, where nematodes were kept in 15°C and 25°C for 24-hour periods, alternating temperatures each day. In this assay, individuals began their thermocycle at 15°C from egg lay.  
Columns:   
Block: experimental block ID number – only 1 block was included here  
Strain: N2 or SKN (skn-1 mutants) denotes the nematode strain  
Treatment: developmental treatments of daf-2 RNAi (daf) or controls (ev)   
Plate.ID: plate ID number – nematodes were housed in plates of 10  
Worm: individual ID number nested within Plate.ID  
Death.Date: date of death  
Cause: cause of death (W = walling, M = matricide, E = exploded, D = natural death, L = lost due to human error)  
D1: start date of experiment  
Age: age (in days) at time of death  
Event: binary variables (1 = yes, 0 = no) for whether natural death occurred (this includes causes D and M)  
Exp: binary variable (1 = yes, 0 = no) for whether an individual exploded (this was included as rate of ‘explosions’ were high – death was counted as an explosion when an individuals cuticle burst)  
Inf:  binary variable (1 = yes, 0 = no) for whether a plate was infected during the assay  

---  
File: Thermo_C_rep.csv  
Reproduction data for N2 and skn-1 mutant nematodes following developmental treatments with daf-2 RNAi or control treatment (ev). A rapid thermocycle was an additional treatment for all individuals, where nematodes were kept in 15°C and 25°C for 24-hour periods, alternating temperatures each day. In this assay, individuals began their thermocycle at 15°C from egg lay.  
Columns:  
ID: individual ID number  
Strain: N2 or SKN (skn-1 mutants) denotes the nematode strain  
Treatment: developmental treatments of daf-2 RNAi (daf) or controls (ev)  
D1-D9: number of offspring produced on given day of adulthood (Days 1 – 9)  
Matricide: binary variable (1 = yes, 0 = no) for whether an individual matricided or not  

---  
File: Thermo_H_LS.csv  
Survival data for N2 and skn-1 mutant nematodes following developmental treatments with daf-2 RNAi or control treatment (ev). A rapid thermocycle was an additional treatment for all individuals, where nematodes were kept in 15°C and 25°C for 24-hour periods, alternating temperatures each day. In this assay, individuals began their thermocycle at 25°C from egg lay.  
Columns:   
Block: experimental block ID number – only 1 block was included here  
Strain: N2 or SKN (skn-1 mutants) denotes the nematode strain  
Treatment: developmental treatments of daf-2 RNAi (daf) or controls (ev)  
Plate.ID: plate ID number – nematodes were housed in plates of 10  
Worm: individual ID number nested within Plate.ID  
Death.Date: date of death  
Cause: cause of death (W = walling, M = matricide, E = exploded, D = natural death, L = lost due to human error)  
D1: start date of experiment  
Age: age (in days) at time of death  
Event: binary variables (1 = yes, 0 = no) for whether natural death occurred (this includes causes D and M)  
Exp: binary variable (1 = yes, 0 = no) for whether an individual exploded (this was included as rate of ‘explosions’ were high – death was counted as an explosion when an individuals cuticle burst)  
Inf:  binary variable (1 = yes, 0 = no) for whether a plate was infected during the assay  

---  
File: Thermo_H_rep.csv  
Reproduction data for N2 and skn-1 mutant nematodes following developmental treatments with daf-2 RNAi or control treatment (ev). A rapid thermocycle was an additional treatment for all individuals, where nematodes were kept in 15°C and 25°C for 24-hour periods, alternating temperatures each day. In this assay, individuals began their thermocycle at 25°C from egg lay.  
Columns:  
ID: individual ID number  
Strain: N2 or SKN (skn-1 mutants) denotes the nematode strain  
Treatment: developmental treatments of daf-2 RNAi (daf) or controls (ev)  
D1-D9: number of offspring produced on given day of adulthood (Days 1 – 9)  
Matricide: binary variable (1 = yes, 0 = no) for 
