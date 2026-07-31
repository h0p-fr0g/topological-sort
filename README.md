# Topological Sort (Generator)

Topological sorting of precedence relations, implemented in vanilla JavaScript. A `Vorrang` class holds the graph and exposes the sort as an ES6 generator (`function*` / `yield`), so the next runnable task is produced on demand.

## Features

- Kahn's algorithm exposed via `Symbol.iterator` as a generator
- Cycle detection (result shorter than the node count means a cycle)
- Small web UI: enter relations as `A -> B` (one per line or comma-separated), get the sorted order
- Built-in test suite (5 cases, including cycles and empty input)

## Running it

No dependencies. Open `topGenerator.html` in any modern browser. The tests run automatically on load — open the browser console to see the results.

## Tech

- Vanilla JavaScript (ES6 generators, `Map`, `Set`)
- HTML / CSS
