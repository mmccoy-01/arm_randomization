This is a `shiny` application that randomizes mice based on their flux values.

## How it works:
The randomization process searches for the seed that has the least amount of variability both between and within groups. The `shiny` app computes a combined metric that accounts for both between-group and within-group variability by using the sum of the standard deviations of the mean total flux between groups and the standard deviations within groups. The 'total_variability' metric is user-defined giving preferential weighting to either the variability between groups or within groups.

## Format of .csv file input:
This is how your columns should be named:
cage_number,	id,	ear_punch,	imaging_date,	total_flux,	avg_radiance

* imaging_date is in ISO 8601 international standard which expresses a day as “2001-02-13” (yyyy-mm-dd)
