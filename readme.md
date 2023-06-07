I was inspired to tinker with partial string match algorithms by the eBird mobile app, which doesn't use one!

I created simple HTML pages to experiment with and compare algorithms in JavaScript.

### Search Page

The `search.html` page runs the final algorithm.  It can be viewed [here](https://philthompson.me/misc/partial-string-match-for-birds/search.html).

### Comparison Page

The `compare.html` page compares results from the algorithms used in development.  It can be viewed [here](https://philthompson.me/misc/partial-string-match-for-birds/compare.html).

### Levenshtein Distance

I implemented the "iterative with full matrix" Levenshtein Distance algorithm from the pseudocode [on Wikipedia](https://en.wikipedia.org/wiki/Levenshtein_distance).

### Bird Lists

For testing, I used eBird's "Printable Checklist" pages.  After saving a page's HTML:

    grep '<div class="subitem">' checklist.html | cut -d '>' -f 2 | cut -d '<' -f 1 | sort > checklist-birds.txt

### License
MIT
