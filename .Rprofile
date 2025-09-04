options(repos=c(CRAM="https://p3m.dev/cran/__linux__/focal/latest",RSPM="https://p3m.dev/cran/__linux__/focal/latest"))

setHook("rstudio.sessionInit", function(newSession) {
  if (newSession)
    message("Welcome to the hands-on part of the Workshop !")
    message("")
    message("Before getting started, please run")
    message("")
    message("  setup_project()")
    message("")
    message("in the R console.")
}, action = "append")

setup_project <- function() {
  if (!require(pak,quietly=TRUE)) {utils::install.packages("pak")}
  if (!require(renv,quietly=TRUE)) {pak::pak("renv")}
  if (!require(admiral,quietly=TRUE)) {pak::pak("admiral@1.1.1")}
}

