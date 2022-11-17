# SGCCA

Here we have all the code related to the analysis presented in the "Functional impact of multi-omic interactions in breast cancer subtypes" by Soledad Ochoa and Enrique Hernández-Lemus
Check https://github.com/mSolEdadO/TCGAmiRmethyRNAIntegration/tree/master/sgcca for history

Order to repeat the analysis  
  1. Get the data into matrixes    
    1.1 getData.R  
    1.2 prepro-mRNA.R  
    1.3 prepro-miRNA.R  
    1.4 prepro-methy.R,   
    1.5 concatena.R  
    1.6 mfa_normi.R  
   2. SGCCA  
    2.1 fit_penalty.R  
    2.2 choose_penalty.R  
    2.3 sgcca.R  
    2.4 sgccaSubsample.R  
    2.5 joinSubsamples.R  
   3. SGCCA functional enrichment  
    3.1 selectedFeatures.R  
    3.2 functions_overrepre.R  
    3.3 functions_overrepre_plots.R  
    3.4 functions_overrepre_groups.R  
    3.5 functionsJaccard.R  
   4. MI networks for the enriched functions  
    4.1 get_matrix.R  
    4.2 https://github.com/CSB-IG/ARACNE-multicore  
        change run.sh because filenames are different  
        line 12 → nom=$(echo $ftsv | cut -d'.' -f 1,2,3)  
        line 23 → n=$( (cd adj; ls) | head -1 | cut -d'.' -f 4 )###check when MI is restricted  
    4.3 MIfilter.R  
    4.4 plotGraph.R  
    4.5 annotateGraph.R  
  
