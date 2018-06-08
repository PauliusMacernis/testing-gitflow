# Testing [Git-flow](https://nvie.com/posts/a-successful-git-branching-model/)
Testing

- Starting the new feature. Once a feature is started, a `feature` branch is created from the current head of `develop`
- Individual commits are made as part of the development of the Features.
    - Ensure that commits constitue a functional unit of work (no partial commits)
    - Ensure that all tests pass
    - Commit message guidelines must be followed:
 ```
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
``` 
```
<type>:
build:      Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)
ci:         Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs)
docs:       Documentation only changes
feat:       A new feature
fix:        A bug fix
perf:       A code change that improves performance
refactor:   A code change that neither fixes a bug nor adds a feature
style:      Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
test:       Adding missing tests or correcting existing tests

```
For example: `feat(universal): add algorithm X into the set of core algorithms`

- On completion, a pull request to develop is created.