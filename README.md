# lineart_01
Lineart defined by coloring areas between lines with various constraints

# Approach Naive
- Pick any line (honestly maybe try using the four frame ones)
- hashmap of all polygons
- link per polygon from all lines defining its border
- Iterate over all other lines and split the area in a before and after intersection
- Modify polygon by iterating over all previous border defining lines and removing those that are now cut off
- Also add the other polygon
