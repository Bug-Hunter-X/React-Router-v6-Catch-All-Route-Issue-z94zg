# React Router v6 Catch-All Route Bug

This repository demonstrates a common issue encountered when using catch-all routes (`/*`) in React Router v6. The catch-all route unintentionally intercepts requests intended for other, more specific routes.

## Problem

The provided `App.js` shows a simple React Router setup.  Despite having routes for `/` and `/about`, the catch-all route (`/*`) is always activated, preventing the other routes from functioning correctly.

## Solution

The `AppSolution.js` demonstrates the solution:  reordering routes. By placing the catch-all route last, React Router correctly prioritizes the other routes before resorting to the fallback. 