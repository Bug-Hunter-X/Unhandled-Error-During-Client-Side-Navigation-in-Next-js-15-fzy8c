# Unhandled Error During Client-Side Navigation in Next.js 15

This repository demonstrates a common error in Next.js 15 applications where an unhandled error during client-side navigation leads to a broken user experience.  The error occurs when navigating to a page that throws an exception.

## Problem
The `pages/about.js` file intentionally throws an error.  In Next.js 15, this error is not gracefully handled, resulting in a blank page or a less-than-ideal error message for the user.

## Solution
The solution involves using `Error Boundaries` to catch errors and display a custom message or fallback component to the user. This provides a much better experience.