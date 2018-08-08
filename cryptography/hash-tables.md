# Hash tables

Hash tables are internally just arrays. The size of the array is typically
smaller than the number of unique values the hash can hold, and so each item in
the array is actually a bucket of values.

Hash tables work by assigning unique numbers to the keys which correspond to
positions (buckets) in the table.

The hashing algorithm can be expected to return the same number given the same
key.

Typically the derived number is greater than the number of spaces in the hash
table, so a modulus calculation is used to return a new number that is within
the lower range. Prime numbers are used because they are less likely to result
in clashes via the modulus calculation.
