# React Router Dom v6 Catch All Route Issue

This repository demonstrates a problem with the catch-all route (`/*`) in React Router Dom v6.  The issue occurs when the catch-all route fails to render when an invalid URL is used, even though other routes are defined. This example shows the issue, as well as a fix for it.  The problem seems to be related to the order and placement of routes, specifically that the catch-all must be last.

## To Reproduce

1. Clone this repository.
2. Install dependencies: `npm install`
3. Run the app: `npm start`
4. Navigate to an invalid URL (e.g., `/invalid-route`).  The `NotFound` component will not render as expected.