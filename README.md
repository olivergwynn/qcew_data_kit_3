# Data Kit - County Quarterly Census of Employment and Wage Filtering
## Version

Current version: 2024-05-28

## Provider

  - Organization: [Mid-Ohio Regional Planning Commission](https://morpc.org)
  - Contact: 
    - Name: Oliver Gwynn
	- E-mail: ogwynn@morpc.org

## Disclaimer

This data kit is a work in progress.

## Introduction

Each quarter the U.S. Bureau of Labor Statistics Census of Employment and Wage produces count of employment and wages reported by employers for the prior quarter. This data set includes annual factors for each given year, average establishment counts and employment levels, total wages, taxable wages and annual contributions, average annual and weekly pay, along with over the year change by count and percentage for each previously mentioned factor. This data kit, slices long-form summarized QCEW data into long-form '.csv's for indivudial variables.

## Outputs
This data kit includes a number of filtered standardized outputs derived from a compilation and trasformation of a set of Quarterly Census of Employment and Wage data from the Bureau of Labor Statistics:

  - For each variable, a long-form table that could (hypothethically) be used to drive a dashboard on the MORPC Insights platform (`./assets/output_data/qcew_quarterly_long_{variable}.csv`)
  
Each output is accompanied by a [Frictionless Resource file](https://specs.frictionlessdata.io/data-resource/), which provides a high-level description of the data and a link to the associated table schema.  The Resource file also provides the [MD5 checksum](https://en.wikipedia.org/wiki/Md5sum) ("hash") and the file size ("bytes") of the data file to allow for integrity checking.

The table schema is described by a [Frictionless Schema file](https://specs.frictionlessdata.io/table-schema/), which describes each of the fields contained in the table, including its name and type, and sometimes provides additional metadata about the table.

## Processes

The outputs are produced by a process which complies and transforms the data:

  1. A fully-automated process implemented as a Jupyter notebook


## Inputs

The process requires inputted BLS QCEW '.csv' files from the user. These files can either be obtained automatically using [qcew_data_kit_2](https://github.com/olivergwynn/qcew_data_kit_2).

  1. Files must come from [qcew_data_kit_2](https://github.com/olivergwynn/qcew_data_kit_2) and placed in input data directory (`./assets/input_data/`)


## Revision history

### 2024-05-28 Oliver Gwynn <ogwynn@morpc.org>

Initial WIP version. 
