# ck3json
Convert CK3 files to JSON

Supports CK3 version 1.2.1

## Usage
```
USAGE:
    ck3json [FLAGS] <file> [grammar]

FLAGS:
    -h, --help         Prints help information
    -m, --melt-only    Melt ck3bin-format and return text without converting to JSON
    -V, --version      Prints version information

ARGS:
    <file>       CK3 file to parse
    <grammar>     [default: ck3txt]  [possible values: ck3txt, ck3bin]
```

# Known issues
- Condition pairs (e.g. `primary_title.tier >= tier_kingdom`) are converted to ordinary pairs, and the type of condition is lost.
- Condition pairs and variables (e.g. `@score = 100`) may be recognised if invalid or not recognised if valid due to the unavailability of a full syntax description of CK3 files.

<!-- Although our dear upstream repository has a cool Crate and has projects using it, we don't. For the reader's sake, we comment out this part of the readme.
## Crate
[![Crates.io](https://img.shields.io/crates/v/ck3json)](https://crates.io/crates/ck3json)

## Projects using ck3json
* [CK3 Family Tree Exporter](https://github.com/blastentwice/CK3-Family-Tree-Exporter-To-Gramps-Fast-JSON-Version) 
-->
