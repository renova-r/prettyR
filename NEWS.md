# prettyR 2.2.3.9001

Renova release, based on CRAN prettyR 2.2-3 (archived on CRAN 2026-04-15).

- `addxtabs()`: the class of the first list element is now compared with
  `identical(class(x[[1]]), "xtab")` instead of `class(x[[1]]) != "xtab"`.
  An element whose class has more than one value (for example a matrix) now
  reaches the intended error message instead of an error in the condition.
  The result for valid `xtab` input is unchanged.
- `R/addxtabs.R` now uses LF line endings (previously CRLF).
- `DESCRIPTION`: `Version` set to `2.2.3.9001`; the stale `MD5` file was
  removed. `COPYING` (GNU GPL, version 2), `README.md` and `NEWS.md` were added.

# Earlier changes (NEWS file of prettyR 2.2-3, unchanged)

```
version 2.2-3

        added significance specification in delim.table

version 2.2-1

	fixed column spacing in print.xtab

version 2.2

	added imports for R CMD check

version 2.1-1

	changed all instances of nchar() to nzchar()

version 2.1

	added a print method for the "describe" function

version 2.0-9

	rewrite of the "describe" family

version 2.0-8

	Add TIFF device to htmlize

version 2.0-7

	Rebuild for R-3.0

version 2.0-6

	nothing really

version 2.0-5

	added the ability to stack a matrix of values to rep_n_stack
	fixed the bug in describe.logical when all values were either TRUE or FALSE

version 2.0-4

	fixed the freq function that I totally screwed up in 2.0-2

version 2.0-3

	removed the deprecated mean(data.frame) call by coercing to matrix
	finally fixed the value name spacing in describe.factor

version 2.0-2

	made decreasing order in freq optional

version 2.0-1

	fixed the right alignment in the decimal.align function
	reformatted the non-HTML tables in print.xtab
	new skew function
	and, of course, it now has a NAMESPACE

version 2.0

	added optional HTML formatting to the xtab function
	added sorting to the freq function
	added the rep_n_stack function to reshape data frames

version 1.9-1

	increased the default spacing for variable names to 20 in describe

version 1.9

	finally fixed the spacing in the column names in print.xtab

version 1.8-9

	I think I've finally fixed the justification in truncString

version 1.8-8

	added the fname.space argument to the describe function

version 1.8-7

	added truncation for long column labels in print.xtab
	added the addxtabs function

version 1.8-6

	fixed the formatting bug in print.xtab that I introduced in version 1.8-5
	added the skew function

version 1.8-5

	More rewriting of the describe family
	added the truncString function

version 1.8-4

	rewriting of the describe family for better formatting

version 1.8-3

	added vertical list output in the describe functions

version 1.8-1

	removed _all_ the \samp tags

version 1.8

	rewrote xtab to return a nested list when more than one table
	  is generated.
	removed \samp tags from \link tags

version 1.7

	added the or (odds ratio) argument to the xtab and print.xtab functions
	 and the automatic display of relative risk.
	fixed the integer overflow in print.xtab (thanks to Harold Baize).
```
