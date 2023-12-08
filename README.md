# DandyWalker_NonCodingMutations
Nour Hanafi's rotation project on non-coding mutations in Dandy-Walker Syndrome.  

Download Encode file from here: https://downloads.wenglab.org/V3/GRCh38-cCREs.bed  
Download ABC file from here: https://mitra.stanford.edu/engreitz/oak/public/Nasser2021/AllPredictions.AvgHiC.ABC0.015.minus150.ForABCPaperV3.txt.gz  

Then run the following in Terminal/command line to get only "brain" elements:  

```bash
grep -E "bipolar_neuron_from_iPSC-ENCODE|H1_Derived_Neuronal_Progenitor_Cultured_Cells-Roadmap|astrocyte-ENCODE" AllPredictions.AvgHiC.ABC0.015.minus150.ForABCPaperV3.txt > AllPredictions.AvgHiC.ABC0.015.minus150.ForABCPaperV3_bipolarneuron_astrocyte_neuronalprogenitor.txt
```

```1.DataCleaning_PreliminaryAnalysis.Rmd``` contains code to take a quick look at cohort and variants. Can be run with either the singleton/duo or trio variant files. Also contains code to run overlaps with ABC enhancers.  


