# thesis_patch-seq
Repository hosts the analysis code for adult patch-seq data of aIP and OP-derived SPNs.

Pipeline:

  1. Processing
  - Creates single cell experiment objects from kallisto outputs
  - Remove low quality cells
  - Normalises data
  - Plots qc metrics

  2. Patchseq QC
   - Calculates microglia contamination scores
   - Plots microglia contamination

  3. DESeq2
   - Zinbwave processing
   - Pseudo-bulk DESeq2 for GFP and RFP neurons
   - Volcano and count plots

  4. Integration
   - Integrates patch-seq dataset with reference dataset
   - Runs integrated dimensionality reduction

  5. Subtype prediction
   - Predicts GFP and RFP neuron subtype with scrattch.hicat
   - Plots predictions
