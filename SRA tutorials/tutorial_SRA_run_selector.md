---
css:
  - css/hero-image.css

# SRA Run Selector Tutorial

The SRA Run Selector is used to take large sets of runs stored in SRA and determine which runs should be used in your analysis.

This tutorial will demonstrate its core functionality, as well as other valuable skills.

**Core functionality:**

- [Find SRA Data in Entrez](#find-sra-data-in-entrez)  
- [Filter an Accession List](#filter-an-accession-list)
- [Get Selected Accession List](#get-selected-accession-list)

**Other valuable skills:**

- [Search for Accessions Data](#search-for-accessions-data)
- [Using the Filters List](#using-the-filters-list)
- [Using the Help Button](#using-the-help-button)

# Core functionality

## Find SRA Data in Entrez

Start by doing a search for brewer's yeast using the organism in Entrez. You can replicate the example search below by clicking [here](https://www.ncbi.nlm.nih.gov/sra/?term=%22saccharomyces+cerevisiae%22%5BOrganism%5D).

<div id="image">
    <img src="images/rst_entrez.png" width=50%>
</div>

- On the left of the search results, click "aligned data" to limit the search to aligned sets.

- From the "Send To" menu, choose "Run Selector".

<div id="image">
    <img src="images/rst_send_to.png" width=50%>
</div>

You will receive a warning that only the first 20,000 experiments are being sent to Run Selector, which is sufficient for this tutorial. In the future, you may want to use additional filters to ensure that more of the 20,000 experiments are of interest to you.

You can learn more about Entrez filters by clicking [here](https://www.ncbi.nlm.nih.gov/books/NBK53591/).

## Filter an Accession List

Run Selector will take a short time to load all the runs into the table. It will also take some more time to show all the available filters on the left side of the page.

<div id="image">
    <img src="images/rst_run_selector_open.png" width=50%>
</div>

Next we will select filters to limit our set of runs to those available in our cloud provider and aligned using the same reference genome.  These filters use metadata supplied by submitters as the terms.  

*Be sure to read all options in a filter list since alternate spellings or capitilization from different submitters can be found in the filters.*

<div id="image">
    <img src="images/rst_filter_selection.png" height=50%>
</div>

- Click the box for DATASTORE provider and AssemblyName to activate these filters.  They will appear as new boxes beneath the Filters List

<div id="image">
    <img src="images/rst_chosen_filters.png" height=50%>
</div>

Select the relevant AssemblyName filter and the DATASTORE provider filter corresponding to your cloud provider. 

The list of runs will now be limited to just those available at the cloud provider you will use, as well as aligned to the chosen reference genome.

## Get Selected Accession List

Now that we have filtered the list of runs, we will add all the filtered runs to our selected list.

Click the blue check box under the "Found Items" flag to add all runs to the selected list.

<div id="image">
    <img src="images/rst_add_selected.png" width=50%>
</div>

This will update the "Selected Row" and allow a cart file or accession list file to be downloaded.

<div id="image">
    <img src="images/rst_added.png" width=50%>
</div>

Click the "Accession List" button to download a text file of the accessions.

# Other valuable skills

## Search for Accessions Data

If you already have a Study (PRJ, SRP) or Sample (SAM, SRS) accession to find data for in SRA, you can use [Run Selector](https://www.ncbi.nlm.nih.gov/Traces/study/?) directly to find the data.

<div id="image">
    <img src="images/rst_search_by_accession.png" width=50%>
</div>


## Using the Filters List

Filters allows us to limit our set of runs to those available in our cloud provider and aligned using the same reference genome.  These filters use metadata supplied both by NCBI and the submitters as the terms.  The Filters List is color coded to indicate the source of the values.  
- Blue text filters are always at the top and are either required metadata or generated by NCBI when the data was processed. 
- Black text filters are from metadata supplied by the submitter in the Run descriptions.  These can be any tag and value pair supplied by the submiters that they felt provided useful information describing the data generation.
- Green text filters are from metadata in the Sample descriptions.  These can be any tag value pair the submitters felt provided useful information describing the sample.

*Be sure to read all options in a filter list because alternate spellings or capitilization from multiple submitters can be found in the filters.*

<div id="image">
    <img src="images/rst_filter_selection.png" height=50%>
</div>

- Click the box for AssemblyName to activate this filter.  It will appear as a new boxe beneath the Filters List

<div id="image">
    <img src="images/rst_chosen_filters.png" height=50%>
</div>

Select the relevant AssemblyName filter and the DATASTORE provider filter corresponding to your cloud provider. 

The list of runs will now be limited to just those available at the cloud provider you will use, as well as aligned to the chosen reference genome.

## Using the Help Button
At the top of the Run Selector page, there is a question mark to the right of the "Run Selector" title.  Clicking this will toggle the help text for the parts of the Run Selector page.

[= top_nav =]

{! _top-nav.md !}

[= mobile_nav =]

{! _mobile-nav.md !}