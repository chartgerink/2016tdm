# Data

The data folder is the folder that is destined to contain all the data. Some good practices are outlined below:

1. The very first raw datafile should *never* be deleted or edited. Make this file read-only to ensure this will not happen (on windows: right click -> properties -> tick "Read only" box; on mac: right click -> get info -> at the bottom, change to "Read only")
2. Ensure that the data are accompanied by an appropriate codebook, if the datafile is not self-explanatory to an outsider.
3. Ensure that the data is available to at least one co-author and that you have a back-up, to ensure data preservation

# Notes per publisher

## BMJ

1. The [TDM policy](https://web.archive.org/web/20160601173953/http://www.bmj.com/company/legal-information/terms-conditions/legal-information/tdm-licencepolicy/) states they are included in Crossref's TDM services, but [Crossref's documentation](https://web.archive.org/web/20160601173957/http://www.crossref.org/tdm/participants.html) does not corroborate. Additionally, BMJ has terms and conditions on the website, which are not in Crossref --- are these included in the login @ Crossref? Did not agree to any terms as far as I know on login.

2. If included in Crossref, then no additional T&C are needed, hence `api_free` coded as 1.

3. Will revisit crossref availability by checking myself.

## Brill

1. No terms and conditions, disclaimer, use policy!

## Cambridge University Press

1. Metadata + abstract API [available](http://journals.cambridge.org/action/stream?pageId=6508&level=2&sessionId=7EB160BCC3547A6FFE9BEE75850E0B6D.journals) with few, minor conditions

2. Archive [available](http://journals.cambridge.org/action/stream?pageId=6508&level=2&sessionId=7EB160BCC3547A6FFE9BEE75850E0B6D.journals) for a certain price.

## Hindawi

1. No TDM policy, but in Crossref. Assuming it is full-text as well, considering their corpus dump is freely available
2. Simply no T&C, so nothing to prohibit I figure
3. Will revisit 1 for crossref.

## IEEE

1. 