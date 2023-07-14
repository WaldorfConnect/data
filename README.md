# WaldorfConnect - data repository

This repository contains `.csv` files with important data used by our systems.
> Comma used as delimieter - first line holds column headers

## schools.csv

The `schools.csv` contains all schools present in our systems (basically all waldorf-assosciated schools in german-speaking countries)

Columns:

- ID (an internal identifier)
- Country (ISO 3166-2)
- School (name of the school)
- StateAssocID (state assosciated identifier, e.g. by the state education board)
- ParentGroupID (group from `groups.csv` "in charge" of this school)

## groups.csv

The `groups.csv` contains all groups and regional assosciations.

Columns:

- ID (an internal identifier)
- Country (ISO 3166-2)
- Name (name of the group)
