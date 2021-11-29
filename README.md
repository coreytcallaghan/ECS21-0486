This repository contains code and data to reproduce Callaghan et al. 2022. Quantifying effort needed to estimate species diversity from citizen science data. Ecosphere.

The data are freely available from eBird here: https://ebird.org/data/download. I used this version: version eBd_May_2020. But the subsetted data for Florida is made available here. I retrieved this data from a SQL database using the script "get_initial_data_from_bigquery.R" which will not be able to be run as one would not have access to this dataset.

The first step would be to run the scripts: "run_grid_analysis_sampling_profile_bootstrapped.R" and "run_grid_analysis_sampling_profile.R" as these produce some large(ish) intermediate files that are not contained here. However, the 'results' folder holds some of the key results.

I provide code and data for 2014-2019, but the manuscript focuses on data from 2019 for presentation and analysis.

If you have any questions, or would like to discuss further, please email me at callaghan.corey.t@gmail.com

These code were run under the following settings:

R version 4.0.3 (2020-10-10)
Platform: x86_64-w64-mingw32/x64 (64-bit)
Running under: Windows Server x64 (build 17763)

Matrix products: default

locale:
[1] LC_COLLATE=English_United States.1252  LC_CTYPE=English_United States.1252    LC_MONETARY=English_United States.1252 LC_NUMERIC=C                          
[5] LC_TIME=English_United States.1252    

attached base packages:
[1] stats     graphics  grDevices utils     datasets  methods   base     

other attached packages:
 [1] mice_3.13.0         vip_0.3.2           pdp_0.7.0           randomForest_4.6-14 GGally_2.1.0        ggcorrplot_0.1.3    tibble_3.0.5        iNEXT_2.0.20       
 [9] lubridate_1.7.9.2   dbplyr_2.0.0        bigrquery_1.3.2     readr_1.4.0         piecewiseSEM_2.1.2  patchwork_1.1.1     sf_0.9-7            scales_1.1.1       
[17] tidyr_1.1.2         ggplot2_3.3.5       dplyr_1.0.3        

loaded via a namespace (and not attached):
 [1] nlme_3.1-149       bit64_4.0.5        RColorBrewer_1.1-2 httr_1.4.2         tools_4.0.3        backports_1.2.1    R6_2.5.0           KernSmooth_2.23-17
 [9] DBI_1.1.1          colorspace_2.0-0   withr_2.4.1        gridExtra_2.3      tidyselect_1.1.0   emmeans_1.5.3      bit_4.0.4          curl_4.3          
[17] compiler_4.0.3     sandwich_3.0-0     classInt_0.4-3     mvtnorm_1.1-1      stringr_1.4.0      digest_0.6.27      foreign_0.8-80     minqa_1.2.4       
[25] rio_0.5.16         pkgconfig_2.0.3    htmltools_0.5.1.1  MuMIn_1.43.17      lme4_1.1-26        htmlwidgets_1.5.3  rlang_0.4.10       readxl_1.3.1      
[33] rstudioapi_0.13    visNetwork_2.0.9   generics_0.1.0     zoo_1.8-8          jsonlite_1.7.2     zip_2.1.1          car_3.0-10         magrittr_2.0.1    
[41] Matrix_1.2-18      Rcpp_1.0.7         munsell_0.5.0      abind_1.4-5        lifecycle_0.2.0    stringi_1.5.3      multcomp_1.4-16    carData_3.0-4     
[49] MASS_7.3-53        plyr_1.8.6         grid_4.0.3         forcats_0.5.0      crayon_1.3.4       lattice_0.20-41    haven_2.3.1        splines_4.0.3     
[57] hms_1.0.0          pillar_1.4.7       boot_1.3-25        estimability_1.3   reshape2_1.4.4     codetools_0.2-16   stats4_4.0.3       glue_1.4.2        
[65] data.table_1.13.6  vctrs_0.3.6        nloptr_1.2.2.2     cellranger_1.1.0   gtable_0.3.0       purrr_0.3.4        reshape_0.8.8      assertthat_0.2.1  
[73] xfun_0.20          openxlsx_4.2.3     xtable_1.8-4       broom_0.7.3        e1071_1.7-4        coda_0.19-4        class_7.3-17       survival_3.2-7    
[81] tinytex_0.29       units_0.6-7        DiagrammeR_1.0.6.1 statmod_1.4.35     TH.data_1.0-10     ellipsis_0.3.1    
