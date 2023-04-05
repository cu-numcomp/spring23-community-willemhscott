# Community Software Analysis Proposal
Please edit this file and push to your repository.

## Software: mpmath

mpmath is a project that has been around for a while in the Python numeric computing community. It is a library for arbitrary precision floating point math that received sponsorship by Google early in its development. It is a dependency of several other major libraries, notably Sympy.

### Stats

| Description | Your answer |
|---------|-----------|
| Repository URL |  https://github.com/mpmath/mpmath  |
| Main/documentation website | https://mpmath.org/  |
| Year project was started | 2007 |
| Number of contributors in the past year | 11 |
| Number of contributors in the lifetime of the project | 44 |
| Number of distinct affiliations | 2-5 |
| Where do development discussions take place? | Github issues or mailing list |
| Typical number of emails/comments per week? |  |
| Typical number of commits per week? | 1-5 |
| Typical commit size | Either less than 10 lines or less than 1000 lines |
| How does the project accept contributions? | Yes, PRs |
| Does the project have an automated test suite? | yes |
| Does the project use continuous integration? | yes/no |
| Are any legal/licensing steps required to contribute? | no or explain below |

### Install and run

Check the following boxes when complete or add a note below if you
encountered a problem.

- [x] I have installed the software
- [x] I have run at least one example
- [x] I have run the test suite
- [ ] The test suite passes

### Notes/concerns/risks

Interestingly, fails a single test, ending up consistently off by a very small factor after running the test several times. The test does pass in the test environment provided by Github.

```
??? >>> fp.chop(fp.quad(lambda t,p: Y1(t,p)*Y2(t,p)*dS(t,p), *sphere))
Expected:
    1.0000000000000007
Got:
    1.0000000000000004

FAILED mpmath/functions/orthogonal.py::mpmath.functions.orthogonal.spherharm
```

All of the other tests pass with no issues.


I wasn't entirely sure how to take the word 'affiliations' in the above questions. There are more than 100 dependent public projects. No other concerns at this time.

#### Note on copyright
Students retain copyright on any work done in completion of a CU
course, so you are authorized to sign a [contributor license
agreement (CLA)](https://en.wikipedia.org/wiki/Contributor_License_Agreement),
affirm a [developer's certificate of
origin (DCO)](https://en.wikipedia.org/wiki/Developer_Certificate_of_Origin),
etc.  If you have concerns about this, please note them and/or reach
out to Jed directly.
