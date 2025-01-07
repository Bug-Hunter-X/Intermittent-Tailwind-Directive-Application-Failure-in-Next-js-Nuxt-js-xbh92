# Intermittent Tailwind Directive Application Failure in Next.js/Nuxt.js

This repository demonstrates a bug where Tailwind CSS directives are not consistently applied in a Next.js/Nuxt.js application. The issue is intermittent and difficult to reproduce reliably. The `bug.js` file contains the problematic code, and `bugSolution.js` offers a potential solution.

## Bug Description

The core problem lies in the inconsistent application of Tailwind CSS classes.  Sometimes, classes are applied correctly, and other times they are ignored, leading to unexpected styling variations or missing styles altogether.  This issue is not consistently reproducible, making debugging challenging.  The problem appears to be related to how the build process interacts with Tailwind's purge mechanism (or similar optimization strategies in Nuxt.js). 

## Reproduction Steps

1. Clone this repository.
2. Install dependencies: `npm install` or `yarn install`.
3. Run the development server: `npm run dev` or `yarn dev`
4. Observe the inconsistencies in styling across different components or page loads. Note the inconsistent application of Tailwind CSS directives.

## Solution

The `bugSolution.js` file offers a potential fix. The exact approach may vary based on your project structure and the specific build process.  It often involves verifying the correct configuration of Tailwind's purge settings or making adjustments to the build process to improve consistency in the application of Tailwind CSS styles.