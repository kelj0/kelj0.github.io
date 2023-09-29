+++
authors = ["Karlo Kegljevic"]
title = "Storage and Retrival"
date = "2023-09-07"
tags = ["storage", "performance", "indexing"]
+++


### Database

On the most fundamental level, a database needs to do two things: when you give it
some data, it should store the data, and when you ask it again later, it should give the
data back to you.
There is a big difference between storage engines that are optimized for transactional workloads 
and those that are optimized for analytics. 


In order to efficiently find the value for a particular key in the database, we need a different 
data structure: an index. An index is an additional structure that is derived from the primary data. 
Many databases allow you to add and remove indexes, and this doesn’t affect the contents of the database; 
it only affects the performance of queries. 
Any kind of index usually slows down writes, because the index also needs to be updated every time 
data is written. 

This is an important trade-off in storage systems: **well-chosen indexes speed up read queries**, 
**but** every index **slows down writes**. For this reason, databases don’t usually
index everything by default, but require you—the application developer or database
administrator—to choose indexes manually, using your knowledge of the application's typical query patterns.

