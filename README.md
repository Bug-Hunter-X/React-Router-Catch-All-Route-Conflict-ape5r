# React Router Catch-All Route Conflict

This repository demonstrates a common issue in React Router v6 where a catch-all route (`/*`) interferes with other, more specific routes.  The problem is that the catch-all route will always match, even before more specific routes have the chance to be evaluated.

The `App.js` file contains the buggy code. The `AppSolution.js` file shows the corrected code.

## Solution

The solution involves carefully ordering the routes in the `Routes` component. More specific routes must be placed *before* the catch-all route.