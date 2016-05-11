---
title: Fetching entries from INSPIRE
---

# Fetching entries from INSPIRE

[INSPIRE](https://inspirehep.net/?ln=en), also known as INSPIRE-HEP, is an open access digital library for the field of high energy physics ([Wikipedia](https://en.wikipedia.org/wiki/INSPIRE-HEP)).

To fetch entries from INSPIRE, choose **Search -&gt; Web search**, and the search interface will appear in the side pane. Select **INSPIRE** in the dropdown menu. To start a search, enter the words of your query, and press **Enter** or the **Fetch** button.

The INSPIRE search function merely passes your search queries onto the INSPIRE web search, so you should build your queries in the same way, except omitting the *find* or *fin* command. This help page will only give a brief introduction to the search queries. More extensive help on searching INSPIRE can be found on the page http://inspirehep.net/info/hep/search-tips .

Your query can be composed of several parts, combined using *and* and *or* as logical operators. Each part is composed of a letter or word indicating the type of field to search, followed by a space and the text to search for.

The following list shows some of the field indicators that can be used:

-   *a* or *author*: search author names
-   *t* or *title*: search in title
-   *j*: journal. Here either the common abbreviation or the 5 letter CODEN abbreviation for a journal can be used. Volume and page can also be included, separated by commas. For instance, *j Phys. Rev.,D54,1* looks in the journal Phys. Rev., volume D54, page 1.
-   *k*: search in keywords

Example queries:

-   *a smith and a jones*: search for references with authors "smith" and "jones"
-   *a smith or a jones*: search for references with either author "smith" or author "jones"
-   *a smith and not t processor*: search for author "smith" and omit references with "processor" in the title
