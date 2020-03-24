# Scraping & Data collection for Covid Testing sites.
Last updated: March 24, 2020

## Current format and column order

Files are stored in CSV format with the follow column order:

`location-name,location-address-street,location-address-locality,location-address-region,location-address-postal-code,location-contact-phone-main,location-contact-url-main,`

[CSV template for this column order](../raw-source-data/2020-03-24-collection-format-template.csv) - obviously use this as a starting point, rename your entries before push and don't overwrite the template.

## Formatting of Fields

- location-name: The proper name of the Medical facility (e.g. Stanford Hospital at 300 Pasteur Drive)
- location-address-street: The proper name of the street as written for USPS mailing, **without commas** (e.g. 4710 Bellaire Blvd. Suite 175)
- location-address-locality: The proper name of the city as written for USPS mailing (e.g. Houston)
- location-address-region: 2 letters capitalized for State (e.g. FL)
- location-address-postal-code: 5 numbers, preceding zeros are kept. (e.g. 07601)
- location-contact-phone-main: 10 numbers, groups of 3 3 4, separated by dashes. No preceding 1 (e.g. 214-555-5555)
- location-contact-url-main: HTTPs when possible, full link to specific site. (e.g. https://subdomain.healthproviderpropername.com/urgent-care/location-name)
