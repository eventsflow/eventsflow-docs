# Commit conventions

## Type

Must be one of the following:

| Type     | Description                                                  |
| -------- | ------------------------------------------------------------ |
| build    | Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm) |
| ci       | Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs) |
| docs     | Documentation only changes                                   |
| feat     | A new feature                                                |
| fix      | A bug fix                                                    |
| perf     | A code change that improves performance                      |
| refactor | A code change that neither fixes a bug nor adds a feature    |
| style    | Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc) |
| test     | Adding missing tests or correcting existing tests            |

## Scope

Possible scope list:
- common: docs/scripts/any related to all components
- eventsflow: core components 
- module/[module-name]: name of affected module

## References

- Conventional Commits 1.0.0, https://www.conventionalcommits.org/en/v1.0.0/
- Contributing to Angular, https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md
