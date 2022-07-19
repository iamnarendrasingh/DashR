# DashR

## Getting started
This package was developed on a Windows 10 operating system, with R version 4.2.1 (2022-06-23), RStudio version 2022.02.0 Build 548 and Rtools40.

* [Link to download the installer for RTools](https://cran.r-project.org/bin/windows/Rtools/rtools40.html)
* [Link to download an R installer from CRAN mirrors](https://cran.r-project.org/mirrors.html)
* [Link to download the installer for RStudio](https://rstudio.com/products/rstudio/download/#download)

For Windows users, it is smoother to install 1) Rtools, 2) R and 3) RStudio in this order.

## Prerequisites

#### ruODK
To install `RuODK`, which is the R client that the `timci` package uses to simply interact with the Application Programming Interface (API) of ODK Central, please follow the instructions below.

#### Installation of ruODK
You can install the latest release of `ruODK` from the
[rOpenSci R-Universe](https://ropensci.r-universe.dev):

```{r r-universe, eval = FALSE}
# Enable the rOpenSci universe
options(repos = c(ropensci = 'https://ropensci.r-universe.dev',
                  CRAN = 'https://cloud.r-project.org'))
install.packages('ruODK')
```
reference : provided [here](https://docs.ropensci.org/ruODK/#install)

#### Update below section

ru_setup(
  svc = "OData Link",
  pid = UpdateNumber,
  fid = "Update Form ID",
  url = "Server URL",
  un =  "UserNamewithEmailAddress",
  pw =  "PASSWORD",
  pp = NULL,
  tz = NULL,
  odkc_version = NULL,
  retries = NULL,
  verbose = NULL,
)
