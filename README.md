# Omeka CSV Datasets

These datasets are provided for learning and testing the CSV Import tools for Omeka: the [plugin for Classic](https://omeka.org/classic/plugins/CsvImport/) and the [module for Omeka S](https://omeka.org/s/modules/CSVImport/).

Files in the **General Datasets** directory should work with both Classic and S.

Files in the **Omeka S** directory have additional columns to make use of some of the additional features in S. These columns are "ID" fields. For example, in the Jane Austen published set there is a column for creator ID so that users can create a Jane Austen item *before* running the import and use the ID column to [import as the resource id for the Jane Austen item](https://omeka.org/s/docs/user-manual/modules/csvimport/#column-options). You can remove these columns and use the files in Omeka Classic.

While some columns will have obvious mappings to Dublin Core and other Omeka vocabularies, other mappings are up to you.

## Files

The following headings correspond to the two directories in this repo. Each paragraph explains the contents and structure of a specific csv file.

### General Datasets

*HolmesCanon*: all of the Sherlock Holmes short stories and novels written by Sir Arthur Conan Doyle. Descriptions and media sourced from Wikipedia. The `File` column has urls to Wikimedia images.

*Cheeses*: a silly csv of cheeses. The `type` and `country of origin` columns could map to a controlled vocabulary. The `milk` column uses `;` for a multi-value separator. The `FileUrl` column has urls to Wikimedia images.

### Omeka S Datasets

*Austen_published:* Jane Austen's published works. Special columns are `creator S id` for resource id and `ref url` which points to the Wikipedia entry for the work.

*heyerMysteries*: Detective novels published by Georgette Heyer. There are no media links in this file. Special columns are `AuthorId`, `Alternative Title`, and `Features` (which gives the name of the recurring detective features in the novel).

## Other Dataset Sources

The following is a far-from-complete list of open source csv datasets of cultural heritage data.

- [British Library free dataset downloads](https://www.bl.uk/collection-metadata/downloads), distributed under a [Creative Commons CCO 1.0 Universal Public Domain Dedication](https://www.bl.uk/about-us/terms-and-conditions/catalogue-datasets-in-rdf-and-csv)
- [Tate Collection](https://github.com/tategallery/collection) dataset from October 2014, released under the Creative Commons Public Domain CC0 licence.
- [MoMA Collection dataset](https://github.com/MuseumofModernArt/collection), distributed with a CC0 license.
- [Library of Congress Selected Datasets](https://www.loc.gov/collections/selected-datasets/about-this-collection/)
