"What is XLOOKUP?" 
If you want to look up a value in Excel, you can use this function. XLOOKUP is a powerful tool that allows you to search a range or array for a specific value and return a corresponding value from another range or array. It simplifies data retrieval and makes your work more efficient.

Why do we need XLOOKUP? 
XLOOKUP is a modern and flexible replacement for older functions like VLOOKUP, HLOOKUP, and LOOKUP. It supports approximate and exact matching, wildcards (* ?) for partial matches, and lookups in vertical or horizontal ranges. This versatility makes it a go-to function for various lookup needs. 🛠️

Syntax of XLOOKUP:
XLOOKUP(lookup_value, lookup_array, return_array, [if_not_found], [match_mode], [search_mode])
• lookup_value: the value that we are looking for in a table.
• lookup_array: the range or array where to search.
• return_array: the range or array from which to return values.

Optional arguments:
• if_not_found: the value to return if no match is found. If omitted, an hashtag#N/A error is returned.
• match_mode: the match type to perform.
 • 0: Exact match.
 • -1: Exact match or next smaller.
 • 1: Exact match or next larger.
 • 2: Wildcard match.
• search_mode: the direction of search
 • 1 (default) - to search from first to last.
 • -1 - to search in reverse order, from last to first.
 • 2 - binary search on data sorted ascending.
 • -2 - binary search on data sorted descending.

Example: In the image, we are looking for the salaries of employees based on their names using the XLOOKUP function.

XLOOKUP(E4, A2:A5, C2:C5,,0)
• E4: the value that we are looking for.
• A2 to A5: The range to look for that value.
• C2 to C5: The array from where to return the value.
• if_not_found: not specified.
• 0: for the exact match.


<img width="1469" alt="XLOOKUP" src="https://github.com/Jaggi0504/XLOOKUP/assets/44519331/db442442-0851-4264-b5a4-9057ee4422ab">
