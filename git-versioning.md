
# Git  Versioning

Versioning follows the pattern of `MAJOR.MINOR.PATCH`

Or more readable would be `[major].[minor].[patch]-[alpha/beta]`  

E.g.   `1.2.0-beta`


Given a version number MAJOR.MINOR.PATCH, increment the:

- `MAJOR`  can be incremented when you make any breaking change, like backward-incompatible API release.

- `MINOR`  is incremented when you add a new feature/functionality and if backward compatible APIs are introduced.

- `PATCH`  is incremented when you make bug fixes


## Commit Messages
Below, pay close attention to the `type` and `body` of the commit messages and based on them either MAJOR/MINOR/PATCH version is incremented.

-   If the  `body`  contains the text “BREAKING CHANGE” then MAJOR version is incremented.
-   If the  `type`  contains feat/feature, then MINOR version is incremented.
-   If the  `type`  contains fix, then PATCH version is incremented.
-   And finally, if the  `type`  contains refactor/style/perf/doc/test/chore, then nothing is increment and no release is made.


### Initial Development:
   -  Major version zero (0.y.z.) is for initial product development.
   - The public API is not stable and software is not production-ready yet.
    
### Pre-release:
   - A pre-release version is for testing that everything is ok and ready to release. This version is still not production-ready.
   - Add a hyphen and identifier at the end of the version number. For example, `1.0.0-alpha.1.` When you need another build, it becomes `1.0.0-alpha.2`.
    
###  Production:
   - When the public API is stable and the product is ready, you can release the major software version (1.y.z).



### References
- https://semver.org/
- (TR)  https://semver.org/lang/tr/
 
