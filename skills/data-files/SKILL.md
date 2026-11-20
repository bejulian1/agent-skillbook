---
name: data-files
description: Create, convert or check CSV, JSON, Markdown and plain text while preserving the meaning of the input.
license: Apache-2.0
---

# Create or convert structured text

Identify the input format, downstream reader and expected encoding. Inspect representative records, including unusual characters, empty fields and identifier formats. Choose how to represent missing values explicitly when the destination loses a distinction the input supports.

- **CSV.** Use a CSV reader and writer for quoting, delimiters, embedded newlines and double quotes. Keep leading-zero identifiers intact. If a spreadsheet will open untrusted text, account for formula interpretation. CSV quoting alone may still produce an executable formula. Keep legitimate numeric values usable and agree on any transformation that changes raw data.
- **JSON.** Use a serializer with finite numbers, valid escapes and the requested record layout. Preserve large identifiers as strings when numeric precision matters. Check whether the consumer expects one JSON value or newline-delimited records.
- **Markdown and plain text.** Preserve the requested heading structure, relative links, line endings and character encoding. Escape table or code delimiters that would change how the content renders.

Reparse structured output and compare record counts, field names, key totals and representative edge cases with the source. Report any lossy conversions and link to the file actually produced.
