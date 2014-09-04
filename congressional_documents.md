---
layout: default
---


* placeholder
{:toc}
s
# Congressional Documents

Currently, this project covers recent documents in the [House Committee Repository](http://docs.house.gov/Committee/Committees.aspx).  

The information is sourced from the bulk data at [github.com/unitedstates](https://github.com/unitedstates/congress). Feel free to [open a ticket](https://github.com/unitedstates/congress/issues/new) with any bugs or suggestions.


## Methods

All requests require a valid [API key](index.html#parameters/api-key), and use the domain:

{% highlight text %}
https://congress.api.sunlightfoundation.com
{% endhighlight %}

### /congressional_documents/search

This collections contains documents from From Congress that are produced through the course of hearings, reports etc. Currently the collection only contains House Committee documents. We hope to add Senate documents and other types of congressional documents in the future.

## Fields

**document_id**
A unique id for each document.

**document_type**
Document types are taken from the House Document type code- "CV": "Committee vote" "WS": "Witness statement", "WT": "Witness truth statement", "WB": "Witness biography", "CR": "Committee report", "BR": "Bill", "FA": "Floor amendment",
"CA": "Committee amendment", "HT": "Transcript", "WD": "Witness document" and "other" is used for all other documents.

**chamber**
house or senate

**committee_id**
ID id a committee is associated with the document

**committee_names**
Full names of the committees associated with the document.

**congress**
Session of Congress.

**house_event_id**
Unique id for each hearing, assigned by the House.

**hearing_type_code**
This discribes if the meeting is a markup, meeting, hearing

**hearing_title**
Title of the hearing associated with the document.

**published_at**
Date and time of publication.

**bill_id**
Bill ID associated with the document. 

**description**
Discription of the hearing.

**version_code**
The short-code for what stage the version of the bill is at. See [GPO](http://www.gpo.gov/help/about_congressional_bills.htm) for explinations for the version code.

**bioguide_id**
Unique identifier for a member of congress if they are associated with the document.

**occurs_at**
Date and time of a hearing associated with the document. 

**urls**
The url is the original link to the document. The permalink is the backup link to the document hosted by the Sunlight Foundation. 

**text**
Extracted text from the document.

**text_preview**
A preview of the text. 

**witness**
Information about a witness associated with a document.

```
	{
		position: "Director",
		witness_type: "Government - State",
		first_name: "Steve",
		organization: "Texas Department of Public Safety",
		middle_name: null,
		last_name: "McCraw"
	},
```