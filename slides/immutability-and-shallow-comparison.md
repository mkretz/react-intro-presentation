*   immutability and shallow comparison
    *   state is always stored in immutable objects
    *   shallow comparison suffices to check for changes in state
    *   deep object traversal never required
    *   updating state means copying whole object
    *   `setState(...)` takes care of immutable update
