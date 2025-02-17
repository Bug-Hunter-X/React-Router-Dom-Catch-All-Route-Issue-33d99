# React Router Dom Catch-All Route Issue

This repository demonstrates a problem with the catch-all route (`/*`) in React Router Dom v6.  The catch-all route unexpectedly intercepts all navigation attempts, even when other routes should be matched. 

## Problem

The `App.js` file contains a simple React Router setup.  The expectation is that navigating to `/` will show the Home component, `/about` will show the About component, and any other route will trigger the NotFound component.  However, only the NotFound component renders. This occurs because the catch-all route `/*` is overly broad and blocks other routes from working correctly.