---
title: Advanced Search
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 18
---

## Advanced Search
Over 90 object record elements can be searched either individually or in combination using the advanced object search. To access the advanced search, click on **Search all objects** in the Objects section on the **SPEC landing page** to navigate to the **Object Search** interface, then click **Advanced search** in the upper right corner to open the advanced search pop-up window.

{: .tip }
> Advanced Search is separate from **Basic Search** and **Use additional search fields** found on the main **Object Search** interface. The advanced search performs a new search; it does not expand or constrain the found set of objects that may appear in the object search result list.

Select a field to search fron the drop down menu and enter or select a search term. Click **+** to add search criteria or the **x** button to remove search criteria, select a **boolean operator** (AND is the default). Optionally, click the gray **(** and **)** to parenthesize a subset of search criteria, turning the parenthesis green. 

The following options appear in the advanced search interface: 

- **Include Inactive Records**:  
  Searches automatically exclude inactive records. Click this check box to include them.

- **Do not include contained objects**:  
  Searches automatically include objects on the shelf and objects contained in other objects. Click this check box to exclude objects contained in other objects.

- **Clear Terms**:  
  Clears all entered values for the fields selected.

- **Reset**:  
  Resets all fields and clears any entered values.

- **Search**:  
  Excute the search. 

{: .tip }
> It may take up to a few minutes for the advanced search to execute, especially if the search criteria results in a very large found set. 

Click the **x** button in the upper right to close the advanced search window without executing the search. Advanced search will remember the user's last search.


## Search Help 

| **To find** | **Type this in the field** | **Examples** |
| Not empty (fields that have data) | \* | \* |
| Empty (fields without data) | = | = | 
| Words that start with specific roman characters (works with fields that use any language except Japanese) | The characters | Chris Smith finds Chris Smith, Smith Chris, Chris Smithson, and Smith Christenson |
| A phrase or sequence of characters that match when they are the first characters in a word (match phrase from word start) | The literal text (characters), including spaces and punctuation, between double quotation marks (") | "Marten and Jones Interiors" finds Marten and Jones Interiors but not Jones and Marten Interiors; "Spring" finds Springville but not ColdSpring Harbor or HotSpring | 
| Words with one or more unknown or variable characters (any one character) | One wildcard character (@) for each unknown character | Gr\@y finds Gray and Grey; @on finds Don and Ron but not Bron |
| Words with zero or more unknown or variable text characters in a row (zero or more characters) | \* for all unknown characters | Jo\*n finds Jon and John; J\*r finds Jr. and Junior; \*phan\* finds Phan and Stephanie; S\* finds Sophie, Steve, and Sven |
| Exact matches of the text you specify (match entire field) | == (two equal signs) for a field content match | ==John finds John but not John Smith; ==John Smith finds John Smith but not Smith, John or John Smithers |
| Exact matches of whole words you specify (match whole word) | = | =Market finds Market, Market Services, and Ongoing Market Research but not Marketing or Supermarket; =Chris =Smith finds Chris Smith or Smith Chris but not Chris or Christopher Smithson |
| A number | The number | .50 finds .5, .50, and $.50 |
| One or more numeric digits | A # character for each digit | # finds 3 but not 30; ## finds 30 but not 3 or 300; #3 finds 53 and 43 but not 3 |
| A date | The date as digits, separated by a valid date separator character (such as a slash or hyphen) | 3/3/2019 finds 3/3/2019, March 3, 2019, and 3-3-2019 |
| Today's date | // | // finds April 4, 2019 (when the current date is 4/4/2019) |
| Any valid value for a date or time component in a date, time, or timestamp | \* or leave component unspecified, while specifying the other components you want to find | 5/12/\* finds the 12th day of May in any year; 5/12 finds the 12th day of May in the current year; \*:15 finds times 15 minutes after any hour; 1/1/\* 7 PM finds timestamps in the 7 o’clock PM hour on January 1st in any year |
| Within the range you specify | .. or ... (two or three periods) | 12:30...17:30      1/1/2019..6/6/2020      A...M |
| Less than a specified value | < \[value] | <40      <9/7/2019      \<M |
| Greater than a specified value | > \[value] | >95129      >9/7/2019      >M |