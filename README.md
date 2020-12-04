# systemic-risk
Some Jupyter notebooks demonstrating various types of models for systemic financial risk, including indicator back-testing, 
network construction, network analytics, statistical stress-testing & economic models. 
Many of these can be run on Azure, when the required R & python packages are supported.  
* https://notebooks.azure.com/ian-buckley/libraries/systemic-risk
* https://github.com/Ian-Buckley/systemic-risk-azure-notebooks  

## Summary table
|Name`   ` |Language`   `|Package`       ` |Author`       ` |Description`       ` |Publication`       ` |
|:----------|:----------|:---------|:----------|:----------|:----------|
[**Py-ABCE--Tutorial.ipynb**](https://notebooks.azure.com/ian-buckley/libraries/systemic-risk/html/Py-ABCE--Tutorial.ipynb)  |Python  |`ABCE`  |Taghawi-Nejad, Davoud  |Agent-based complete economy tutorial.  |**+** Taghawi-Nejad, Davoud, Rudy H. Tanin, R. Maria Del Rio Chanona, Adrián Carro, J. Doyne Farmer, Torsten Heinrich, Juan Sabuco, and Mika J. Straka. “ABCE: A Python Library for Economic Agent-Based Modeling.” In International Conference on Social Informatics, 17–30. Springer, 2017.
[**Py-neva--Network-based-stress-testing.ipynb**](https://notebooks.azure.com/ian-buckley/libraries/systemic-risk/html/Py-neva--Network-based-stress-testing.ipynb)  |Python  |`neva`  |Bardoscia, Marco  | Network valuation in financial systems.  Neva values equities of banks that hold cross-holding of debt. Several known contagion algorithms (e.g. Furfine, Eisenberg and Noe, and Linear DebtRank) are special cases of Neva.   |**+**  Barucca, Paolo, Marco Bardoscia, Fabio Caccioli, Marco D’Errico, Gabriele Visentin, Stefano Battiston, and Guido Caldarelli. “Network Valuation in Financial Systems.” SSRN Scholarly Paper. Rochester, NY: Social Science Research Network, June 14, 2016. http://papers.ssrn.com/abstract=2795583.
[**Py-sfc_models.ipynb**](https://notebooks.azure.com/ian-buckley/libraries/systemic-risk/html/Py-sfc_models.ipynb)  |Python  |`sfc_models`  |Romanchuk, Brian  |Stock-Flow Consistent (SFC) models in Python  |**+** Romanchuk, Brian. An Introduction to SFC Models Using Python. BondEconomics, 2017.  https://www.amazon.ca/Introduction-SFC-Models-Using-Python/dp/0994748094. 
[**R-ccgarch.ipynb**](https://notebooks.azure.com/ian-buckley/libraries/systemic-risk/html/R-ccgarch.ipynb)  |R  |`ccgarch`  |Nakatani, Tomoaki  |Conditional Correlation GARCH models. Required for MES & SRISK measures.  |**+** Nakatani, Tomoaki. Ccgarch: Conditional Correlation GARCH Models, 2014. https://cran.r-project.org/web/packages/ccgarch/index.html.  
[**R-mFilter.ipynb**](https://notebooks.azure.com/ian-buckley/libraries/systemic-risk/html/R-mFilter.ipynb)  |R  |`mFilter`  |Balcilar, Mehmet  |Miscellaneous time series filters e.g. for detrending financial time-series such as (early warning) indicators for systemic risk.  |**+** Balcilar, Mehmet. MFilter: Miscellaneous Time Series Filters (version 0.1-3), 2007. https://cran.r-project.org/web/packages/mFilter/index.html.
[**R-systemicrisk--Bayesian-network-reconstruction.ipynb**](https://notebooks.azure.com/ian-buckley/libraries/systemic-risk/html/R-systemicrisk--Bayesian-network-reconstruction.ipynb)  |R  |`systemicrisk`  |Gandy, Axel  |A toolbox for systemic risk based on liabilities matrices. A Bayesian approach to estimate the liabilities matrices where only row and column sums of the liabilities matrix. Alternative to entropic & other point estimate approaches.  |**+** Gandy, Axel. CRAN - Package Systemicrisk. Accessed September 11, 2016. https://cran.r-project.org/web/packages/systemicrisk/index.html.
[**Sheppard--Python-for-econometrics--Example_GJR-GARCH.ipynb**](https://notebooks.azure.com/ian-buckley/libraries/systemic-risk/html/Sheppard--Python-for-econometrics--Example_GJR-GARCH.ipynb)  |Python  |`-`  |Sheppard, Kevin  |The example Estimating the Parameters of a GARCH Model, from Sheppards book: Python for Economics.   Estimate the parameters of a GJR-GARCH(1,1,1) model by optimizing the log-likelihood function (quasi-maximum likelihood) with a constant mean.  |**+** Sheppard, Kevin. Python for Econometrics, 2017. https://www.kevinsheppard.com/Python_for_Econometrics.
[**Eikon-API-Proxy.ipynb**](https://notebooks.azure.com/ian-buckley/libraries/systemic-risk/html/Local/Eikon-API-Proxy.ipynb)  |Python  |`eikon`  |  |Python scripts to request data from Thomson Reuters Eikon.  |




**WORK IN PROGRESS**

### Interesting notebooks & tutorials in finance & economics
#### Python
* https://github.com/rsvp/fecon235
* https://www.kevinsheppard.com/Python_for_Econometrics
* https://www.quantopian.com/tutorials
* http://tpq.io/ 
#### R
* https://cran.r-project.org/web/views/Finance.html
* http://statisticalestimation.blogspot.ca/2016/09/blog-post.html
