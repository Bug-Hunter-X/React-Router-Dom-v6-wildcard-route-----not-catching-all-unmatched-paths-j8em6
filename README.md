This repository demonstrates a bug in React Router DOM v6 where the wildcard route '*' does not match all unmatched paths as expected. The issue is specifically related to how the Routes component handles path matching when nested routes are involved. The solution involves using the exact prop in the child route component. 

## Bug:

The bug is present in the `bug.js` file where the wildcard route `/` is not catching all unmatched paths. For instance, attempting to navigate to a non-existent path will not render the NotFound component.

## Solution:

The solution is shown in `bugSolution.js`, where the issue is fixed by using the exact prop in the child route component.