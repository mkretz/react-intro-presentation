## Testing

*   Unit testing framework of choice is Jest (https://facebook.github.io/jest/)
    *   Behaviour-driven DSL very similar to Jasmine
    *   offers snapshot testing based on React virtual DOM
        *   each test execution captures rendered output
        *   next test execution can compare output to previous execution
