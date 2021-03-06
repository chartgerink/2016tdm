# Text- and Data Mining (TDM) case study

The CrossRef API participants are retrieved from [here](http://www.crossref.org/tdm/participants.html) and [here](http://tdmsupport.crossref.org/). Springer and TaylorFrancis are only represented in the second link, which is odd.

## Information retrieval

A three-step approach was used in the coding. Step 1 included collection of resources, whereas step 2 pertains to the coding of these resources. 

Step 1 pertains to the variables `publisher`,
`url`,
`open_access`,
`contact`,
`whois`,
`terms_conditions_url`,
`crossref_tdm`,
`crossref_tdm_clickthrough`. These variables were resource variables and could be readily coded without much time effort or potential to interpretation.  

Step 2 requires some more interpretative elements to the resources collected in Step 1. This pertains to the variables `api`,
`api_unrestricted`,
`terms_conditions_scrape`,
`nc_terms_conditions_scrape`,
`terms_conditions_spider`,
`nc_terms_conditions_spider`,
`tdm_policy`,
`lit_dump`,
`lit_dump_unrestricted`,
`lit_dump_policy`. As such, these were coded separate from Step 1 to clearly demarcate the objective elements from more interpretative elements. As such, the coding remains accountable and verifiable. To this end, notes will be kept per coded publisher to provide details.

Step 3 includes emailing the publishers to verify or disconfirm the codings.

INCLUDE TEMPLATE EMAIL HERE

### Coding protocol

1. Open Terms and Conditions link
2. Save page to wayback machine
3. Open hypothes.is
4. Annotate parts containing information on scraping in yellow, use CTRL+F for keywords "scrap", "download", "automat", "bot", "spider" to identify key sections.
5. Code whether a specific country's copyright applies in the terms and conditions `copyright_law_country` (country acronym, + denotes whether it adds a modifier to include "other countries")
6. Code whether the user is allowed, based on the T&C, to download articles for research purposes. If scraping is not forbidden, it is seen as allowed.
7. Code `terms_conditions_scrape`, 0 = explicit statement forbidding scraping, 1 = no explicit statement forbidding scraping, NA = states nothing about scraping.
8. Code `nc_terms_conditions_scrape`, 0 = forbids scraping for non-commercial/does not make a distinction, 1 = allows scraping specifically for non-commercial activities, NA = nothing coded for `terms_condition_scrape` so nothing possible.
9. Code `terms_conditions_spider` similarly to #5.
10. Code `nc_terms_conditions_spider` similar to #6.
11. Use the site's websearch to look for a tdm policy with the term "tdm policy", "mining", "tdm". Only inspect first page for relevant hits pertaining to a tdm policy. If found, copy the url to the policy into the spreadsheet under variable `tdm_policy`.
12. Code `api` availability, 0 = no, 1 = yes, NA = is no info found (note that if available in `crossref_tdm`, this automatically converts to a yes)
13. Code `api_free`, where 0 = restrictions, 1 = free (i.e., one does not need to make an account or accept conditions to use API), NA = if no API available. Note that if there is an agreement in CrossRef, this is seen as restricted.
14. Use the websearch for "corpus", "dump", "subset" (based on how PMC calls their dump), "full-text", "fulltext"
15. Add whether the downloads are freely available in `lit_dump_free`, 0 = restriction (e.g., login), 1 = free, NA = no dump available
16. If there is a policy available on the download page, add the link to the policy in `lit_dump_policy`.

All of the links included in the spreadsheet will be archived at the Wayback Archive for persistence. A duplicate spreadsheet will be included that provides these links in case they are required in the future.