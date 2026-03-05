# Useful RegEx

```\burl\b( (?==)|\b(?!\s*=))``` matches the word "url" when it is not followed by an equal sign, or when it is followed by an equal sign but not preceded by a whitespace character. This can be useful for finding instances of "url" that are not part of a keyword argument, especially for refactoring. This works for any word, just replace "url" with the desired word.

```\(\d{3}\) ?\d{3}-\d{4}``` matches a phone nunber in format (123)123-4567 or (123) 123-4567

```\b\d{5}\b``` matches a 5 digit zip code, but not a 9 digit zip code (12345-6789)

```\b\d{5}-\d{4}\b``` matches a 9 digit zip code, but not a 5 digit zip code (12345-6789)

```\b\d{5}(-\d{4})?\b``` matches both 5 and 9 digit zip codes (12345 or 12345-6789)

```\b\d{3}-\d{2}-\d{4}\b``` matches a social security number in format 123-45-6789

```^\d{4}-(0[1-9]|1[0-2])-(0[1-9]|[12]\d|3[01])$``` matches a date in format YYYY-MM-DD, ISO 8601 format

```^\$\d+(\.\d{2})?$``` matches a price in format $123.45 or $123
