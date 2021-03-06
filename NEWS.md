# snpEnrichment 1.8.0

## Minor improvements and fixes
* In `R/*estimate_ethnicity*.R`, 
    + use tidy style.
* In `DESCRIPTION`, 
    + a little change in Title and Description to clearly state the package uses a sampling approach.
    + setup package to use roxygen2.

# snpEnrichment 1.7.0
* NAMESPACE: Update to fix warnings from R CMD check using R version 3.2.2.
* DESCRIPTION: Update according to new imports in NAMESPACE.

# snpEnrichment 1.6.6
* NAMESPACE: Update to fix warnings from R CMD check using R version 3.2.2.
* R/enrichment.R: Update 'plot' method to fix global definition warnings.

# snpEnrichment 1.6.5
* tests/RUN-TEST_snpEnrichment.R: Add a test script.

# snpEnrichment 1.6.4
* R/enrichment.R: Update 'getEnrichSNP' to add information about related eSNP for xSNP.

# snpEnrichment 1.6.3
* DESCRIPTION: Change maintainer email.
* R/enrichment.R: Minor changes.

# snpEnrichment 1.6.2
* R/enrichment.R: Minor changes.
* R/chromosome.R: Minor changes.
* R/Global.R: Minor changes.

# snpEnrichment 1.6.1
* R/enrichment.R: Minor changes.

# snpEnrichment 1.6.0
* R/Global.R: Fix a bug in 'compareEnrichment' method with parameter 'empiricPvalue=TRUE'.

# snpEnrichment 1.5.10
* R/Global.R: Fix a glitch in 'readEnrichment'. Sometimes chromosomes 10 and 20 are read respectively instead of 1 and 2.
* R/Global.R: Some minor changes.

# snpEnrichment 1.5.9
* data/toyEnrichment.RData: Minor changes.
* R/Global.R: Add internal function '.splitByChrom'. 
    User is now allowed to use a single file in 'snpListDir' for 'readEnrichment' function.
* man/snpEnrichment-internal.Rd: Update according to R code changes.
* man/readEnrichment.Rd: Update according to R code changes.

# snpEnrichment  1.5.8
* R/enrichment.R: Update 'print' method to print results according to the parameter 'empiricPvalue' in 'reSample' function.
* R/enrichment.R: Update 'compareEnrichment' according to changes in 'print' method.
* R/chromosome.R: Some minor changes.
* man/compareEnrichment.Rd: Update according to R code changes.
* man/print-methods.Rd: Update according to R code changes.

# snpEnrichment 1.5.7
* R/*.R: Add function 'getEnrichSNP' and some minor corrections.
* man/*.Rd: Update according to R code changes and some corrections.
* NAMESPACE: Updata according to R code changes.
* inst/example.R: Update 'excludeFile' list according to changes in 'toyEnrichment' and 'extdata'.
* man/snpEnrichment-package.Rd: Update 'excludeFile' list according to changes in 'toyEnrichment' and 'extdata'.
* man/excludeSNP-methods.Rd: Update 'excludeFile' list according to changes in 'toyEnrichment' and 'extdata'.
* README.md: Update 'excludeFile' list according to changes in 'toyEnrichment' and 'extdata'.

# snpEnrichment 1.5.6
* R/Global.R: 'readEnrichment' works with at least one snp list in 'snpListDir'.
* R/Global.R: Fix 'mclapply2' under operating systems which are not Linux.
* R/Global.R: Fix 'maxCores' under operating systems which are not Linux.
* man/snpEnrichment-package.Rd: Update example.
* inst/example.R: Update according to changes in 'snpEnrichment-package.Rd'.
* README.md: Update according to changes in 'snpEnrichment-package.Rd'.
* R/*.R: the "types" parameter is renamed "type".
* man/*.Rd: Update according to R code changes.

# snpEnrichment 1.5.5
* man/*.Rd: Replace 'summary' by 'print'.
* inst/example.R: Replace 'summary' by 'print' according to changes in '*.Rd' files.
* README.md: Replace 'summary' by 'print' according to changes in '*.Rd' files.

# snpEnrichment 1.5.4
* R/*.R: Change default value for 'empiricPvalue' parameter to 'TRUE'.
* man/*.Rd: Update according to R code changes.
* inst/example.R: Update according to R code changes.
* README.md: Update according to R code changes.
* R/enrichment.R: Change warning messages in 'compareEnrichment'.

# snpEnrichment is 1.5.3
* R/Global.R: Fix an issue under Windows systems with mclapply
* R/Global.R: Update warning message in 'reSample' method.
* R/Global.R: Fix an issue in 'initFiles', 'writeLD' and 'readEnrichment'.
    Some bim files could not found according to the sorting method in the folder.
* R/enrichment.R: 'plot' method is consitent with parameters used in 'reSample' (e.g. 'empiricPvalue')
* README.md: Some corrections.
* R/*.R: Change default value for 'onlyGenome' parameter to 'TRUE'.
* man/*.Rd: Update according to R code changes.

# snpEnrichment 1.5.2
* R/Global.R: Add some internal functions to check files needed by 'initFiles', 'writeLD' and 'readEnrichment' functions.
* man/snpEnrichment-internal.Rd: Update according to R code changes.
* inst/example.R: Update according to R code changes.

# snpEnrichment 1.5.1
* R/Global.R: Internal function 'maxCores' handle warnings on macintosh system.
* R/Global.R: Handle warning / error in 'initFiles' when 'snpInfoDir' or 'signalFile' are missing or invalid.

# snpEnrichment 1.5.0
* R/Global.R: Fix a bug in 'compareEnich' when 'xSNP' was missing in "object.*".
* man/*.Rd: Some corrections in example.

# snpEnrichment 1.4.3
* man/*.Rd: Update according to R code changes.

# snpEnrichment 1.4.2
* R/enrichment.R: Fix a bug when 'xSNP' field is empty in 'plot' method.
* R/Global.R: Fix 'options(stringsAsFactors=FALSE)' in 'writeLD'.
* man/snpEnrichment-package.Rd: Update according to DESCRIPTION file.

# snpEnrichment 1.4.1
* R/*.R: Minor optimizations.
* R/enrichment.R: Fix a bug in 'plot' method with 'ggplot=TRUE'.

# snpEnrichment 1.4.0
* R/Global.R: Change internal functions used by 'readEnrichment' and 'writeLD'.
* R/Global.R: Improvment in 'writeLD' function.
* R/Global.R: Add 'depth' parameter in 'writeLD' function.
* R/Global.R: Minor optimizations.
* R/enrichment.R: Fix a bug when 'object' was not updated properly, with 'reSample' function and all defaults parameters.
* R/*.R: Remove 'extendMethod' parameters from all functions.
* data/: Remove 'toyEnrichmentM2.RData'.
* data/: Rename 'toyEnrichmentM1.RData' to 'toyEnrichment.RData'
* man/*.Rd: Update according to R code changes.

# snpEnrichment 1.3.12
* R/*.R: Minor changes in R code.
* R/Global.R: Remove parameter 'snpListDir' in 'initFiles' function.
* R/Global.R: Fix 'ldThresh' parameter in 'initFiles' function.
* man/*.Rd: Update according to R code changes.

# snpEnrichment 1.3.11
* R/enrichment.R: Add 'pvalue' parameters in 'plot' method.
* R/plot-methods.Rd: Update according to R code changes.

# snpEnrichment 1.3.10
* R/*.R: Add 'empiricPvalue' arguments in order to choose if p-values should be empirical
    or based on null distribution (resampling).

# snpEnrichment 1.3.9
* R/Enrichment.R: Prevent a bug in 'plot' method with 'ggplot=TRUE'.

# snpEnrichment 1.3.8
* R/*.R: Minor changes in R code.
* R/Global.R: Fix a missing square root in Z statistics computation.
* R/enrichment.R: Fix legend position in 'plot' for 'ggplot=TRUE'.

# snpEnrichment 1.3.7
* R/*.R: Minor changes in R code.
* R/Global.R: Change p-value computation in '.reSample' and 'compareEnrich' functions.
* R/Global.R: Convergence control on Z statistic is removed in '.reSample' and 'compareEnrich' functions.

# snpEnrichment 1.3.6
* R/*.R: Minor changes in R code.
* R/enrichment.R: 'compareEnrichment' now returns 'object.x', 'object.y' and object from comparison.
* R/compareEnrichment.Rd: Update according to R code changes.

# snpEnrichment 1.3.5
* R/*.R: Minor changes in R code.
* R/enrichment.R: Fix an error in 'reSample' method that occurs in 'compareEnrichment' method.
* R/enrichment.R: Add controls on installed packages for 'ggplot=TRUE' in plot method.
* R/enrichment.R: Remove convergence control in 'reSample' when 'Resampling' slot are empty in 'compareEnrichment'.
    'compareEnrichment' now performs 'nSample' resampling for 'object.x', 'object.y' and for comparison.
* R/global.R: Remove 'while' loop in '.compareEnrich' (not used yet).

# snpEnrichment 1.3.4
* R/*.R: Minor changes in R code.
* man/compareEnrichment.Rd: Add alias for signature "Enrichment".

# snpEnrichment 1.3.3
* R/enrichment.R: Fix a bug in 'excludeSNP' when 'LD' is set to 'FALSE'.

# snpEnrichment 1.3.2
* R/enrichment.R: Redefine 'print' method for 'Enrichment' object.
* R/chromosome.R: Redefine 'print' method for 'Chromosome' object.

# snpEnrichment 1.3.1
* R/Global.R: 'readEnrichment' returns an error when 'initFiles' was not run before.
* R/enrichment.R: 'reSample' method for 'Enrichment' object now reruns one warning when 'mc.cores' is decreased.
* R/enrichment.R: call for 'reSample' method is saved properly in 'Enrichment' object.
* R/enrichment.R: Redefine 'plot' method for 'Enrichment' object. 'plot' method can use ggplot2, if 'ggplot' is set to 'TRUE'.
* man/*.Rd: Update documentations files according to R code modification.

# snpEnrichment 1.3.0
* R/Global.R: 'readEnrichment' can deal with ld files computed with plink directly.

# snpEnrichment 1.2.3
* man/EnrichSNP-class.Rd: Add alias for method '[' and '[' with signature = 'EnrichSNP,ANY,ANY,ANY'.
* man/Chromosome-class.Rd: Add alias for method '[' and '[' with signature = 'Chromosome,ANY,ANY,ANY'.
* man/Enrichment-class.Rd: Add alias for method '[' and '[' with signature = 'Enrichment,ANY,ANY,ANY'.
* R/Global.R: Now use 'read.plink', 'col.summary', 'ld' from 'snpStats' package for read plink files and compute MAF and LD.
* R/Enrichment.R: Fix 'show' method in order to deal with new parameters in 'readEnrichment' and 'reSample' functions.
* R/*.R: Change default setting for 'mc.cores' to 1.
* man/*.Rd: Update documentations files according to R code modification.

# snpEnrichment 1.2.2
* R/*.R: Change name of 'SNP' class to 'EnrichSNP'.
* R/*.R: Some improvements and computation time optimisations.
* R/Global.R: Add 'ldDir' parameter in 'writeLD' which allow to choose the directory where LD files should be written.
* R/Global.R: Add 'ldDir' parameter in 'readEnrichment'.
* R/Global.R: 'initFiles' now write and clean tempory files used by 'readEnrichment'.
* R/Global.R: Now LD is only computed by 'writeLD'. Not anymore by 'initFiles'.
* R/Global.R: Remove 'ldThresh' and 'LD' parameters from 'initFiles'.
* R/Global.R: Remove 'signalFile', 'transcriptFile', 'snpInfoDir', 'distThresh', 'LD',
    'ldThresh', 'sigThresh', 'MAFpool' and 'extendMethod' parameters from 'compareEnrichment'.
* R/enrichment.R: Remove 'signalFile', 'transcriptFile', 'snpInfoDir', 'distThresh', 'LD',
    'ldThresh', 'sigThresh', 'MAFpool' and 'extendMethod' parameters from 'compareEnrichment'.
* R/enrichment.R: Fix issue for the whole genome convergence plot in 'plot' methods. Add parameter 'onlyGenome'.
* man/*.Rd: Update documentations files according to R code modification.

# snpEnrichment 1.2.1
* R/*-class.R: Add 'print' methods (same as 'show').
* R/Global.R: Add error messages when files can not be created by 'initFiles'.
* R/Global.R: Remove 'require(parallel)' from 'mclapply2' function.
* exdata/*: Move all external data to 'inst' directory in order to be used in examples.
* man/*.Rd: Update documentations files according to R code modification.

# snpEnrichment 1.2.0
* R/enrichment.R: Add 'onlyGenome' parameter, which allow to compute the resampling step at chromosome level and genome or only at genome level.
* R/enrichment.R: Fix 'plot' methods for low number of resampling.
* R/enrichment.R: Change 'Parameters' to "Call".
* R/enrichment.R: 'show' is available for 'Call' slot.
* R/enrichment.R: Remove 'sigThresh' and 'extendMethod' parameters from "reSample" method with 'signature="Enrichment"'.
* R/enrichment.R: Remove 'sigThresh' and 'extendMethod' parameters from "excludeSNP" methods.
* R/enrichment.R: Fix abscisse according to 'nSample'. Abscisse origin is now equal to three.
* R/enrichment.R: 'chrNumber' is replaced by 'chr', in 'plot' method for 'Enrichment' object.
* R/Global.R: Fix bug in 'compareEnrichment' when some fields were not reseted with the option 'onlyGenome=TRUE'.
* R/Global.R: Remove 'onlySignal' parameter from 'writeLD' function.
* R/Global.R: Change 'Parameters' to "Call".
* R/Global.R: Remove 'sigThresh' and 'extendMethod' parameters from "excludeSNP" methods.
* NAMESPACE: Fix 'NAMESPACE' with missing 'SNP' class and methods.
* data/*: Generate new toy datasets.
* extdata/*: Generate new external datasets (iles needed to run the examples for the packages functions).
* man/*.Rd: Update documentations files according to R code modification.

# snpEnrichment 1.1.4
* R/enrichment.R: Now results from method 'compareEnrichment' are the enrichment object and the summary table.
* R/enrichment.R: 'nSample' in 'excludeSNP' can be equal to 0.
* R/Global.R: 'maxCores' return at least 1.
* R/mclapply2.R: run in parallel mode with at least 1 core.

# snpEnrichment 1.1.3
* R/Global.R: Some improvements and changes of functions: 'initFiles', '.writeSignal', 'writeLD'.

# snpEnrichment 1.1.2
* R/Global.R: Add informations about snp losses on each step of the algorithm.
* R/Global.R: Fix minor bugs in read functions.

# snpEnrichment 1.1.1
* man/plot-methods.Rd: Corrects the description of method plot.

# snpEnrichment 1.1.0
* R/Global.R: Some minor code optimization and simplification.
* R/Global.R:  The method 'excludeSNP' now exclude the extended list of SNP provided in 'excludeFile'.
    Note: 'excludeFile' can be a character vector with SNPs or a file path which contains a SNPs list.
* R/Global.R: The function 'writeLD' now compute Linkage Disequilibrium for all SNPs in reference data or only for SNPs in signal.
* R/enrichment.R: The slot 'Signal' of Enrichment object is replaced by slot 'Loss'. This slot gives information about data losses (e.g. SNPs removed).
* R/Global.R: Add 'plot' method for Enrichment object. This method show the convergence of Z statistics.
    Z statistic is scaled and centered in order to compare the convergence in chromosomes/genome.
* R/Global.R: Fix a bug where some SNP which are not in reference data ('snpInfoDir') were not extended with SNP in LD.
* R/Global.R: Fix bug for the extend method 'LD block' where SNPs which are not in linkage with another SNP, are removed.
* man/*.Rd: Update Rd files with the R code correction.

# snpEnrichment 1.0.2
* R/Global.R: Matrix or data.frame are not anymore evaluated in the slot 'Parameters' of Enrichment object.
* R/enrichment.R: Fix errors that occurred when the SNP list is too low in 'reSample' function.
* R/enrichment.R: Fix an error that occured in 'compareEnrichment', when non-resampled Enrichment objects are given in the list fields.

# snpEnrichment 1.0.1
* R/Global.R: Some minor code optimization and simplification.
* R/enrichment.R: The method 'summary' is not anymore masked by loading 'snpEnrichment' package.
