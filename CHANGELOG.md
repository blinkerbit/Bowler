## v0.9.0

* Added `bowler test` command for testing codemod scripts (#82)
* Added `python_version` option to load files with Python 2 print statement (#123)
* Implemented `Query.encapsulate()` to generate `@property` wrappers (#113)
* Improvements to `Query.add_argument()` and positional arguments (#104)
* No longer depends on shelling-out to `patch` command for applying diffs (#120)
* Fix `Query.write()` to be non-interactive and silent (#88)
* Fix unexpected error code after successful queries (#89)
* Marked package as typed for PEP 561 support (#124)
* Improved documentation (#100)

```bash
$ git shortlog -sn v0.8.0...
    13  John Reese
    12  Tim Hatch
     5  Anentropic
     5  David Arnold
     3  Marion
     2  Mohit Solanki
     2  ajberchek
     1  Kamil Breguła
```

## v0.8.0

* Bug fix: reverify using fissix instead of ast to preserve the ability to modify code
  that is incompatible with the host version of python (#78)
* Log full traceback of errors during `bowler run` (#86)
* Adds a maintainers guide (#83)
* Changes `filename_matcher` to receive a full path, in case it needs to read
  the file separately (#81)
* Adds `query_func` to BowlerTestCase making it easier to test the provided
  helpers, and improve exception capture in tests.

```bash
$ git shortlog -sn v0.7.1...
     6  Tim Hatch
     5  John Reese
     1  Andy Freeland
     1  Mariatta
     1  Mariatta Wijaya
```

## v0.7.1

* Bug fix: skip writing files if they fail to parse after transform (#76)
* Improved debug logging for parse failures (#75)

```bash
$ git shortlog -sn v0.7.0...
     4  John Reese
     1  Tim Hatch
```

## v0.7.0

* Validate transformed AST before generating diff or writing changes (#26)
* Improve function argument modifiers to not require filters (#29)
* Better support for renaming dotted module names (#61, #72)
* Materialize file list before deciding how many processes to create (#70)
* Multiple documentation and site fixes (#50, #54, #55, #60)
* Debug mode now runs in a single process (#53)
* More test cases for helpers (#57)
* Build wheel distributions during release (#67, #71)
* Start tracking code coverage and upload results to coveralls.io (#71)
* Mark Bowler as requiring Python >= 3.6 (#71)

```bash
$ git shortlog -sn v0.6.0...
    26  John Reese
     5  Bojan Mihelac
     5  Leopold Talirz
     2  Tim Hatch
     1  Guru
     1  Philip Jameson
     1  peng weikang
```

## v0.6.0

* Fix matching for functions with more than one decorators (#10)
* Fix matching function/method calls preceded by the `await` keyword (#6)
* Fix silent failures when processing files without trailing newlines (#20)
* Better patching behavior for large files with many hunks (#21)
* Support passing `pathlib.Path` values to `Query()` (#23)
* Fix interactive mode when IPython not available (#31)
* Better error logging and debugging (#38, #39)
* Support refactoring arbitrary file extensions (#37)
* Better testing framework and more unit tests (#43)
* New helpers for numeric type inference (#42)
* Support returning leaf/node elements from modifiers (#14, #44)
* Fix lint/type checking on Python 3.7+ (#45)
* Fixes and improvements to documentation (#13, #30, #32)
* Consistent shebang/copyright headers in source files (#24, #25, #33)

```bash
$ git shortlog -sn v0.5.1...
    22  John Reese
    18  Tim Hatch
     8  Lisa Roach
     3  Syrus Akbary
     1  Sadie Bartholomew
     1  Bruno Oliveira
     1  Łukasz Langa
     1  Christian Delahousse
     1  Loren Carvalho
     1  Qingzhuo Aw Young
```
