# Useful RegEx

```\burl\b( (?==)|\b(?!\s*=))``` matches the word "url" when it is not followed by an equal sign, or when it is followed by an equal sign but not preceded by a whitespace character. This can be useful for finding instances of "url" that are not part of a keyword argument, especially for refactoring. This works for any word, just replace "url" with the desired word.

```\(\d{3}\) ?\d{3}-\d{4}``` matches a phone nunber in format (123)123-4567 or (123) 123-4567