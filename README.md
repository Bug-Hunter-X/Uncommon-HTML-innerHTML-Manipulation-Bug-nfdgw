# Uncommon HTML Bug: Repeated innerHTML Manipulation

This repository demonstrates a subtle but important issue related to repeatedly modifying the `innerHTML` property of an HTML element. Directly manipulating `innerHTML` in a loop or repeatedly can lead to performance problems and unexpected behavior, particularly in large or complex documents. The example shows how directly modifying `innerHTML` repeatedly can degrade performance. The solution provides a more performant and reliable method for updating HTML.

## Bug
The file `bug.html` shows an example where directly modifying `innerHTML` appends a paragraph to the div. This approach becomes inefficient if this operation is repeated many times.

## Solution
The file `bugSolution.html` demonstrates a better approach using `createElement` and `appendChild`, illustrating a more efficient approach that avoids the performance overhead of manipulating `innerHTML` repeatedly.