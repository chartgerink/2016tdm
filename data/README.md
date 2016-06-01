# Data

The data folder is the folder that is destined to contain all the data. Some good practices are outlined below:

1. The very first raw datafile should *never* be deleted or edited. Make this file read-only to ensure this will not happen (on windows: right click -> properties -> tick "Read only" box; on mac: right click -> get info -> at the bottom, change to "Read only")
2. Ensure that the data are accompanied by an appropriate codebook, if the datafile is not self-explanatory to an outsider.
3. Ensure that the data is available to at least one co-author and that you have a back-up, to ensure data preservation

# Notes per publisher

## BMJ

1. The [TDM policy](https://web.archive.org/web/20160601173953/http://www.bmj.com/company/legal-information/terms-conditions/legal-information/tdm-licencepolicy/) states they are included in Crossref's TDM services, but [Crossref's documentation](https://web.archive.org/web/20160601173957/http://www.crossref.org/tdm/participants.html) does not corroborate. Additionally, BMJ has terms and conditions on the website, which are not in Crossref --- are these included in the login @ Crossref? Did not agree to any terms as far as I know on login.

2. If included in Crossref, then no additional T&C are needed, hence `api_free` coded as 1.