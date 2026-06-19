---
type: Article
title: "Data Structures And Objects"
description: ""
resource: "authors/virtual_adrianco/blogger_perfcap_posts/Data_structures_and_objects.txt"
tags:
  - article
---

# Data Structures And Objects






## Excerpt

Title: Data structures and objects
URL: https://perfcap.blogspot.com/2005/03/data-structures-and-objects.html

The exacct data file is a complex tagged object format that is read via the libexacct library routines. While generic and flexible, it is a pain to get at the data. There are two demo programs that display the information, I used /usr/demo/libexacct/exdump to print out the information shown earlier, and there is also a perl library and a script called dumpexacct.pl. It displays the tags and types like this:<br /><br /><pre><br />GROUP<br />  Catalog = EXT_GROUP|EXC_DEFAULT|EXD_GROUP_PROC<br />  ITEM<br />    Catalog = EXT_UINT32|EXC_DEFAULT|EXD_PROC_PID<br />    Value = 1904<br />  ITEM<br />    Catalog = EXT_UINT32|EXC_DEFAULT|EXD_PROC_UID<br />    Value = 25<br />...<br /></pre><br /><br />I used this information to define a data structure that will be populated with the data from the file as the first processing step. I left the tags as comments, and defined reasonable amounts of fixed space for strings. The task and flow structures are similar.<br /><br /><pre><br />struct ex_proc { // EXT_GROUP|EXC_DEFAULT|EXD_GROUP_PROC<br /> uint32_t pid;  // EXT_UINT32|EXC_DEFAULT|
...


## Sources

[1] Source file: authors/virtual_adrianco/blogger_perfcap_posts/Data_structures_and_objects.txt
