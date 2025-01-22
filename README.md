# Next.js 15 App Router: Error when no layout exists

This repository demonstrates a bug in Next.js 15's App Router where an error is thrown when no layout exists in the `pages` directory.  The application should gracefully render without a layout if none is explicitly defined.

## Bug Description

When using the App Router in Next.js 15, if the `pages` directory does not contain a layout file (e.g., `layout.js`), the application fails to render and throws an error.  This behavior is unexpected and prevents users from having minimal project setups without a default layout.

## Reproduction Steps

1. Create a new Next.js 15 app using the App Router.
2. Remove the layout file from the `pages` directory (or don't create one).
3. Run the development server and observe the error.

## Expected Behavior

The application should render the default page content without a layout or throw a more user-friendly error message.

## Actual Behavior

The application throws an error and fails to render. This can lead to unexpected behavior and hinders development.
