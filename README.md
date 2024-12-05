# Next.js 15 App Router Trailing Slash Issue

This repository demonstrates a bug in Next.js 15's App Router related to handling trailing slashes in links. When navigating to a route with a trailing slash, unexpected behavior occurs. The `/about` route works fine but adding `/about/`  causes issues.

## Bug Description:

The issue is observed when using the `<Link>` component with a path that includes a trailing slash. While navigating to `/about` functions correctly, attempting to navigate to `/about/` leads to errors or unexpected rendering. 

## Solution:

The solution involves ensuring your routes are consistently handled and not attempting to load two similar paths that will cause conflict or use a different method for handling trailing slashes within the router.