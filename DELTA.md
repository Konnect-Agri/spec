# Delta in the Spec





## Our Thought process
- Identify what things we need as top level elements and not tags or xinput (LoanApplicationDoc Schema)
- Identify why this is not possible/good to do via tags or xinput
- Identify if it is a generic enough cross domain use case to be submitted as a RFC to the `core` Beckn spec,
else we can look at an adaptation of Beckn, something on the lines of `DSEP`
- Map the new entries into the APIs
- Submit the RFC
- Fight for it!!!!!


## Thought board

- Should the spec be more generic towards the finance sector in general or just mortgages?
- Should only think about mortgages where things are sanctioned with a collateral, or should we also think about personal loans?

Trying to solve this problem incrementally, by first identifying and mapping the Odisha agri loan use case and then trying to generalise it.


## Approach

1. Go through those sheets and try to figure out an exhaustive (90%+ coverage) list of attributes that are required for the finance sector.
2. Map those to the core spec directly, figure out what can be mapped directly, what is acceptable as tags and XInput, what we absolutely want as first class citizens
3. Add those items as first class citizens, and get the `ADAPTED` spec reviewed by Ravi and team.


## Open Questions

1. Do we think in terms for finance and fintech, or do think in terms of loans only, if loans do we include all types of loans or just mortgages.

## APIs

### `search`:

- This is fine (for the most part), might need schema mapping incase of loan products, that can be checked at last,
but tags and xinput should suffice the use case, and will check later

### `select`:

- This is where the application form comes into the picture and we think the order object is not adequate to fulfil those needs.
- try to map the loan application document fields in the order object again, if not then create the loan application doc  

### `init`

### `confirm`
### `track`
### `update`

### `cancel`