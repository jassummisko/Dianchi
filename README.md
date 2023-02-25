# Dianchi - Batteries for Yuescript

This is a Yuescript library serving to provide functions one would commonly expect to see in a standard library.

The following modules are currently available:
### `functools` - Functions commonly used in functional programming.
```moon
"Name   Args          Description"
----------------------------------
take    table, n      -- Return first n elements of table
drop    table, n      -- Return table with first n elements removed
head    table         -- Return first element of table
tail    table         -- Return all but first element of table
map     table, f      -- Return table with function f applied to each element
foldl   table, f, v   -- Fold table from left to right with function f and starting from value v
foldr   table, f, v   -- Like foldl, but right to left
fold    table, f      -- Equivalent to foldl (tail table), f, (head table)
sum     table         -- Return sum of table
product table         -- Return product of table
reverse table         -- Return table in reverse order
sorted  table(, f)    -- Return sorted table with func as f as an optional key function
```

### `checkertools` - Functions commonly used to check for truth values.
```moon
"Name   Args          Description"
----------------------------------
any     table         -- Returns true if any of the elements are true, otherwise returns false
all     table         -- Returns true if all of the elements are true, otherwise returns false
```

### `strtools` - Common string manupulation functions
```moon
"Name   Args          Description"
----------------------------------
split   string, spr   -- Returns table of string split into substrings by separator spr.
words   string        -- Returns table of string split into words.
chars   string        -- Returns table of each character of string.
join    table(, sep)  -- Concatenates all strings of table with sep in between, then returns the concatenated string; sep defaults to space if left empty. 
```

### `misc` - Miscellaneous
```moon
"Name     Args    Description"
----------------------------------
importAll table   -- Imports all elements of table into global scope
```
