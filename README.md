# MultiMR
MultiMR is an R package designed to streamline the process of conducting Mendelian Randomization (MR) analyses across multiple exposures and outcomes simultaneously. Built on top of the popular TwoSampleMR package, MultiMR integrates essential diagnostic tools to ensure robust and reliable MR results.

### Key Features:
> 1) &nbsp; Simultaneous Analysis: Perform MR analysis for multiple exposure-outcome pairs in a single run.
> 2) &nbsp; Heterogeneity and Pleiotropy Tests: Easily evaluate heterogeneity and horizontal pleiotropy using built-in methods.
> 3) &nbsp; Outlier Detection: Automatically detect and handle outliers using the radial package.
> 4) &nbsp; User-Friendly Interface: Intuitive functions and well-documented workflows for users at all levels.
> 5) &nbsp; Efficient and Comprehensive: Obtain detailed results, including effect estimates, heterogeneity statistics, and pleiotropy measures, all in one place.

### Installation
To install MultiMR, download the package from this GitHub repository and run the following command in R:
    
    install.packages("MultiMR_0.1.0.tar.gz", repos = NULL, type = "source")

### Usage
Here's an example of how to run a multi-exposure and multi-outcome MR analysis using MultiMR:
  
  Load the MultiMR package

  install.packages("MultiMR_0.1.0.tar.gz", repos = NULL, type = "source")
  
  library(MultiMR)
  
  Conduct MR analysis for multiple exposures and outcomes
  results <- multi_mr_analysis(
                  exposures = list("ieu-a-299" = "Lipid Levels", 
                                   "ieu-a-300" = "Blood Pressure"),
                  outcomes = list("ieu-a-2" = "Coronary Artery Disease", 
                                   "ebi-a-GCST009541" = "Heart Failure"))

### View the results
print(results)

### Contributions and Issues
Contributions, suggestions, and bug reports are welcome! Feel free to open an issue or submit a pull request to help improve MultiMR.
