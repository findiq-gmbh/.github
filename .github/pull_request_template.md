
## Scope
- [ ] Is the purpose of the PR clear?
- [ ] Is the scope of the PR appropriate? (less than 500 line changes)

## Code Quality
- [ ] Is the code easy to understand?
- [ ] Are functions/classes well-named and serve a single purpose?
- [ ] Is the code properly modularized? (clear destinction between database, files, helpers and routes)

## Documentation
- [ ] Are documentation and code comments clear and useful?
- [ ] Are examples added in the documentation?
  - docstrings / jsdoc
- [ ] Is external documentation updated?
  - Readmes in Github
  - Permissions and roles in Notion
  - Architecture and processes in Notion

## Functionality
- [ ] Are edge cases accounted for?
- [ ] Is there any impact on existing functionality?
  - Are there breaking changes between FE and BE (changes in the OpenAPI-Spec?)
- [ ] Is the new feature modularized and can be deactivated?
  - E.g. feature-flags set?

## Performance
- [ ] Are there any obvious performance concerns?
  - DB indicies set correctly?
- [ ] Are there potential problems with async code?
  - Is blocking code introduced in non-blocking paths?
  - Is there thread starvation or overloading of services?(aka asyncio gather of beanie actions)
- [ ] Are there possible race-conditions?

## Testing
- [ ] Are there tests for new code?
- [ ] Do they cover edge cases?

## Dependencies
- [ ] Are there new dependencies introduced? If so, are they necessary and justified?
  - Are they without copyleft?
- [ ] Are new external services introduced? If so, are they necessary and justified?
  - Are error paths and health checks handled correctly?

## Security
- [ ] Are there any potential security vulnerabilities?
  - Are there changes related to the permission or role systems and do they adhere to our defined principles?
- [ ] Does the code handle sensitive information appropriately?
  - E.g.: logging of user data
