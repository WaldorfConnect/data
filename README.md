# WaldorfConnect - data repository

This repository contains `.csv` files with important data used by our systems.
> Comma used as delimiter - first line holds column headers

# Image folder

The `img` folder holds all assets image related to database entities. 
Subfolders are `group` for group related images and `school` for school related images.

The underlying folder structure follows the following scheme:

- `1` (primary key of the entity the images are attached to) 
  - `logo.png` (The logo of the associated entity)
  - `image.png` (An immersive picture of the associated entity)

### Disclaimer on copyrights

We can only accept images that were published which are:

- taken by yourself
- under a free license (e.g. via Wikimedia Commons)
- rightfully obtained with *written* consent by the author

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

The `groups.csv` contains all groups.

Columns:

- `id` (an internal identifier)
- `region_id` (foreign key of region the group is located in)
- `name` (group name)
- `name` (short descriptive text)

## regions.csv

The `regions.csv` contains all regions and regional assosciations.

Columns:

- `id` (an internal identifier)
- `name` (name of the region)
- `iso_code` (ISO 3166-1 or ISO 3166-2 code)
- `supervisor_group_id` (foreign key of group supervising this region)
