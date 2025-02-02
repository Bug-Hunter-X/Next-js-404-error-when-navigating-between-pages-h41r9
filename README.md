# Next.js 404 Error Reproduction

This repository demonstrates a common Next.js issue where a 404 error occurs when navigating to a page using the `Link` component, even when the page file exists in the `pages` directory.

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install` to install the necessary dependencies.
3. Run `npm run dev` to start the development server.
4. Navigate to the home page (`http://localhost:3000`).
5. Click the link to go to the '/about' page.

You'll notice a 404 error is thrown.

## Solution

The solution involves ensuring the about.js file is correctly placed in the pages directory, and that the export default function in About.js is correct. In the example this error is present due to a typo in the filename.

This repository provides both the buggy code and the corrected code for comparison.