# General 

## What makes a sustainable architecture?
1. `Patterns`: Architecture, state management, abstractions
2. `Processes`: Code reviews, blueprints, design, documents
3. `Systems`: Testing infastructure, static analysis, build systems

Start with the bottom requirements with `Systems` and work towards `Patterns`

## Tooling
* `Programming Language`: TypeScript
* `Front-End Library`: React
* `Testing Tools`: Testing Library, Vitest, Playwright

## Testing Notes - End Goal is to close the feedback loop for the Development Team

### Specturm of testing - Apply what works with the Environment and the Team 
`Unit` => `Component` => `End-to-End`

* `Unit`: 
    - Smallest possible test you can make in the program. It deals with inputs and outputs and checks to see if the output is the result that was to be expected

* `Component` middle ground for `Unit` and `Integration`: 
    - Testing out an individual UI component in our application

* `Integration Tests` Realistic `End-to-End` test: 
    - One or more units for testing. That pokes the entire application from the User's perspective

* `End-to-End` Un-Realistic: 
    - Biggest test that is from the Users perspectiv. This is the ideal end goal of the feature that is being tested (i.e. Client => Server => Database) (tigerbeetle database does a good job at this by creating virtual enviroments that could mimic all possible variables)