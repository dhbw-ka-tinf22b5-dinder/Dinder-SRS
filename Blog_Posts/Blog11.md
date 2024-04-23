# Clean Code Refactoring

## Refactoring
### Frontend
- Mostly using biome.js, it caught errors in:
  - mostly imports
    - sorting by alphabet
    - declare TypeScript class imports with "type"
  - formatting
  - redundancy
    - e.g. semicolons, which are mostly optional in JavaScript, which is the cause for no other checker marking this as an error
  - too many or missing spaces in nested functions, making it unclear in which level of nesting the code is supposed to be in
  - `'` being used instead of `"`

### Backend
- Usage of Spring Profiles
- In-Memory Database (H2) for local tests, depending on the profile
    - now, an internet connection is optional to run the application
    - testing out changes without affecting the production database
- Database Connection configuration was changed from a custom bean to using the Spring autoconfiguration
- Flyway is also now loaded using the autoconfiguration
- The `AuthorityFactory` was renamed to `AuthoritySupplier` to better reflect the purpose of the interface

## Further changes
### Backend
- Research and testing for storing images in Supabase Storage
- Some endpoints were added, for example for receiving information about advertisements
