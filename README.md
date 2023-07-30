# WaldorfConnect - data repository

This repository contains `.csv` files with important data used by our systems.
> Comma used as delimiter - first line holds column headers

## schools.csv

The `schools.csv` contains all schools present in our systems (basically all waldorf-assosciated schools in german-speaking countries)

Columns:

- `id` (an internal identifier)
- `name` (full school name)
- `short_name` (shorted school name, e. g. `Rudolf-Steiner-Schule` turns into `RSS`)
- `region_id` (foreign key of region the school is located in)
- `address` (geographic address of the school)
- `email_bureau` (mail address of the school management/bureau)
- `email_smv` (mail address of the school council/SMV)
- `state_id` (state assosciated identifier, e.g. by the state education board)

## groups.csv

The `groups.csv` contains all groups and regional assosciations.

Columns:

- `id` (an internal identifier)
- `region_id` (foreign key of region the group is located in)
- `name` (group name)
- `name` (short descriptive text)
