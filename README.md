# React Router v6 Nested Routes Issue

This repository demonstrates a common issue encountered when using nested routes with the wildcard route (`/*`) in React Router v6.  The wildcard route unintentionally intercepts all routes, preventing nested routes from functioning correctly.

## Problem Description

The provided code uses nested routes.  However, the `/*` wildcard route always takes precedence, resulting in the `NoMatch` component rendering even when a nested route should be active.

## Solution

The solution involves restructuring the routes to prevent the wildcard route from overshadowing the nested routes. The order and specificity of the routes are crucial to resolving this issue.