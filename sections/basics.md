[<<< Previous](key-terms.md) | [Next >>>](cleanup.md)

# Regex Basics

To begin, we are going to use [the online tool regexr](https://regexr.com/). Explore the interface, what do you notice? What are the different sections of the interface?

## Building blocks

![XKCD Regex Comic](http://b.yu8.us/xkcd-1171-perl_problems.png)

Regex goes deep! Finding it all a little perplexing is the only right response. The original point was to describe states of mathematical "automata" in the most compact, condensed way possible. Not for mere mortals just trying to do their work. However, with a little patience, it really is boundless what all you can accomplish. Easier tools definitely exist for specific purposes, but there are few tools that are as flexible and transferable across interfaces and use cases with no programming required.

- **Delimiters** are not always visible but worth making explicit: All regular expressions need delimiters to denote where they begin and end.
- **Characters** describe literal string matches.
    - Non-printing characters
    - Escaping characters
- **Character classes** describe categories including digits, words, spaces, or all of the things.
    - `\d` (`\D`)
    - `\w` (`\W`)
    - `\s` (`\S`)
    - `.`
- **Anchors** describe whether in the beginning or end of a line.
    - `^`, `$`
- **Character sets** help group valid matches, when you want to match on OR another.
    - `[]`
- **Quantifiers** describe how many of preceding character or character set.
    - `{}`
    - `*` (Kleene star)
    - `+`
    - `?` (:palm_tree: keep it laaaazy :palm_tree:)
- :underage: **Capture groups and references** group matching strings so you can refer to them on the fly, either in the search itself or during find-and-replace. :underage:
    - `()`
    - `$1`
    - `\1`

## Do try it at home

1) Download the text of the [Swarthmore Phoenix (October 15, 1918)](../data/phoenix-ocr-1918-10-15.txt).
2) Open it in Visual Studio Code.
3) Select the search icon in the left sidebar.

How would you find:

- Years?
- Students and Alumni?
- Quotes?
- Headlines and advertisements?