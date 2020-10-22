# DATA 512 A1: Bias in data
## Goals:
The goal of this assignment is to construct, analyze, and publish a dataset of monthly traffic on English Wikipedia from January 1 2008 through August 30 2020.

## Data Source:
Liscence : [MIT](https://github.com/ankitapal189/data-512/blob/main/data-512-a1/LICENSE.md)<BR>
Terms of Use : https://www.mediawiki.org/wiki/Wikimedia_REST_API#Terms_and_conditions<BR>
 <BR>
 We used 2 APIs:<BR>
1.The Legacy Pagecounts API ([Documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts), [Endpoint](https://wikimedia.org/api/rest_v1/#!/Pagecounts_data_(legacy)/get_metrics_legacy_pagecounts_aggregate_project_access_site_granularity_start_end))
December 2007 - July 2016.<BR>
2.The Pageviews API  ([Documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews), [Endpoint](https://wikimedia.org/api/rest_v1/#!/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end))
July 2015 - August 2020<BR>

## Describe the values of fields in the final data file:
| Column | Description |
|--------|-------------|
| Year | Year|
| Month | Month|			
| pageview_desktop_views | Desktop traffic as recorded by Pageviews API  |
| pageview_mobile_views | Mobile traffic as recorded by Pageviews API  |
| pagecount_desktop_views | Desktop traffic as recorded by Legacy Pagecounts API |
| pagecount_mobile_views |  Mobile traffic as recorded by Legacy Pagecounts API   |
| pageview_all_views | Total traffic as recorded by Pageviews API |
| pagecount_all_views | Total traffic as recorded by Legacy Pagecounts API |

## Known issues or special considerations with the data that would be useful for another researcher to know :
1. The date ranges for each API and overlapping date ranges are very useful to knpw. <BR>
2. Data from the Pageview API excludes spiders/crawlers, while data from the Pagecounts API does not. <BR>
3. Due to mismatching ranges. We need to replace 0 for the date ranges where API does not provide the relevant data
