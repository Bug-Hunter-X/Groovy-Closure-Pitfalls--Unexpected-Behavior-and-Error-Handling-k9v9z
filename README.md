# Groovy Closure Pitfalls

This repository demonstrates some uncommon yet important error scenarios related to using closures in Groovy. Closures, while powerful, can lead to subtle bugs if not handled carefully.  This example focuses on argument mismatches, unhandled exceptions, and concurrency issues.

## Issues Addressed

* **Argument Mismatch:** Incorrect number of arguments passed to a closure can result in unexpected behavior or exceptions.
* **Unhandled Exceptions:** Exceptions within closures might not be caught by outer `try-catch` blocks, requiring explicit handling within the closure itself or employing more robust techniques like `try-catch` inside closure.
* **Concurrency Issues:** Using closures in multithreaded environments requires careful consideration of synchronization to prevent race conditions.
* **Delegate Property Usage:** Demonstrates potential problems with the `delegate` property and scope.

## How to Run

1. Clone the repository.
2. Run the `bug.groovy` script to observe the unexpected behavior.
3. Examine `bugSolution.groovy` for improved and safer handling of closures.