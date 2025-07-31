# Searching

# Linear search

The simplest method of searching a dataset, and often called a ‘serial’ search

- Starting at the beginning of the dataset, each item is examined until a match is made
- When found, the search ends
- If there is no match, the search will end

# Binary search

The fast search algorithm that works on the principle of ‘divide and conquer’

But the biggest drawback of this is… the data **must** be fully sorted

The search is repeatedly divided in half

if the value of the middle terms are checked and depending if the value being looked for is in the left or right half, the half that the answer is not in is removed.

This continues until the answer is found, or if there is no value it stops at the closest value