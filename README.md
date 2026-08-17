# DTSA 5301 — Final Projects

Two reproducible R Markdown analyses from CU Boulder DTSA 5301 (Data Science as a Field).
Each pulls its own data straight from the source, so both knit end to end with no local files.

### Does Danger Rise After Dark? Temporal Patterns in NYPD Shooting Incidents
`nypd_shooting_time_patterns.Rmd`

Tests whether the common belief that risk climbs through the night actually shows up in the
data, first across time of day and then across time of year. Uses the NYPD shooting incident
dataset from NYC Open Data, read live from their API. Written with tidyverse.

### Less Deadly, or Just Better Counted? The U.S. COVID-19 Case-Fatality Ratio Over Time
`covid19_report.Rmd`

Tracks the U.S. case-fatality ratio from January 2020 to March 2023 to ask whether COVID-19
genuinely became less lethal or whether case detection simply improved, then models the
relationship between cases and deaths across states. Data from the Johns Hopkins CSSE
repository. Written in base R only — no external packages.

## Running them

```r
install.packages("rmarkdown")      # plus "tidyverse" for the NYPD report
rmarkdown::render("covid19_report.Rmd")
```

## License

MIT
