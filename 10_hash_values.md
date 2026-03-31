# 10 Hash values
- 40 characters that are unique - alphanumeric (a-f)(0-9)
- generated together from data + some hash value
- this is the mechanism for data integrity
- sometimes referred as "SHA", each commit references the commit before it
- if you change the chain somewhere all the following commits must also change
- if you have the same data you will get the same SHA even from files from different locations
- you get data integrity
- the algorithm is called SHA-1
- each commit references the commit that precedes it, can't just be modified without consequences for the following commits