# Regex Tips and Tricks

## Preamble

These examples and exercises pertain to the .NET flavor of Regex, which is what we use in Magnet AXIOM.

## Talking Points

* Regex is complex.
* Use case in forensics.
* .NET Regex vs. other variants.
* Advanced searches and column filters in AXIOM.
* Regex testers.
* Universal Truth about Regex.
* Interest in more Regex content?

## Mock Dataset

If you would like to use the same dataset as in the exercise, you can download them here:

[Mock SQLite Dataset from Mockaroo](https://github.com/forensicmike/magnet-regex-tips-tricks/blob/gh-pages/mock_data/mock_data.sqlite)

[Custom Artifact for AXIOM](https://github.com/forensicmike/magnet-regex-tips-tricks/blob/gh-pages/mock_data/mock_data_artifact.xml)

## Teaching Points

* String and word boundaries with \b, ^, and $
* Escaping special characters
* Grouping and the use of Logical 'Or'
* Numbers and letters'es, anchoring
* Quantifiers - the specific and the indefinite

## Quick Reference

This reference guide lists some common .NET regex constructs, particularly the ones covered in the Tips and Tricks session on August 13.

| Construct   | Usage                                                                                                           |
|-------------|-----------------------------------------------------------------------------------------------------------------|
| [123]       | Matches any single character matching 1, 2, or 3.                                                               |
| [123]{5}    | Matches exactly 5 consecutive characters matching 1, 2, or 3.                                                   |
| [abc]{3,6}  | Matches between 3 to 6 consecutive characters matching a, b, or c.                                              |
| [def]{3,}   | Matches atleast 3 consecutive characters matching d, e, or f.                                                   |
| [0-9]*      | Matches zero or more numeric digits between 0-9.                                                                |
| [0-9]+      | Matches one or more numeric digits between 0-9.                                                                 |
| [A-Z]s?$    | Matches any character A-Z, optionally including an 's' before the end of the string.                            |
| ^(one\|two) | Matches the word one or two at the beginning of the string.                                                     |
| \bsearch\b  | Matches the word search but only when it is between word boundaries (spaces, punctuation, start or end of line) |
| [\w\W]*?    | Mike's Favorite - Match an indefinite number of, well, anything, terminating at the earliest opportunity.       |


## Links

* [Regex Keyword examples](https://www.magnetforensics.com/blog/using-keywords-with-magnet-axiom/) - Magnet blog by [Jamie McQuaid](https://twitter.com/reccetech)

* [Keywords for PII in Magnet AXIOM](https://www.magnetforensics.com/blog/keywords-for-personally-identifiable-information-pii-in-magnet-axiom/) - Magnet blog by [Tarah Melton](https://twitter.com/melton_tarah)

* [.NET Regular Expression Language Quick Reference](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expression-language-quick-reference) - from Microsoft

* [Character Escapes in .NET Regular Expressions](https://docs.microsoft.com/en-us/dotnet/standard/base-types/character-escapes-in-regular-expressions) - from Microsoft

* [Regex Hero](http://regexstorm.net/tester) - .NET Regex Tester

* [Mockaroo](https://www.mockaroo.com) (fantastic website used for mock test data generation)
