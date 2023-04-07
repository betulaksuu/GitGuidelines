# Commit Message Guidelines#

Format: `<type>: <subject>`

## Example

```
feat: add hat wobble
^--^  ^------------^
|     |
|     +-> Summary in present tense.
|
+-------> Type: chore, docs, feat, fix, refactor, style, or test.
```


Types:

- `build`: Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)
- `ci`: Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs)
- `docs`: Documentation only changes
- `feat`: A new feature
- `fix`: A bug fix
- `perf`: A code change that improves performance
- `refactor`: A code change that neither fixes a bug nor adds a feature
- `style`: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
- `test`: Adding missing tests or correcting existing tests

**Good**

- feat: improve performance with lazy load implementation for images
- chore: update npm dependency to latest version
- Fix bug preventing users from submitting the subscribe form
- Update incorrect client phone number within footer body per client request

**Bad**

- fixed bug on landing page
- Changed style
- oops
- I think I fixed it this time?
- empty commit messages

References:

- https://www.gitkraken.com/learn/git/best-practices/git-commit-message
- https://www.conventionalcommits.org/ 
- https://www.conventionalcommits.org/tr/
- http://karma-runner.github.io/1.0/dev/git-commit-msg.html
- https://www.freecodecamp.org/news/how-to-write-better-git-commit-messages/

Examples

- https://github.com/amzn/style-dictionary
