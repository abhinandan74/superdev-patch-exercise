# Patch Notes

## Summary of Changes

- Fixed incorrect task filtering by grouping the title/description search conditions in the backend SQL query.
- Updated the matching Oracle SQL reference queries to keep the filtering logic consistent.
- Removed the artificial `Thread.sleep()` query delay from `TaskController.java`.
- Fixed pagination so changing the search query or status filter resets the page to 1.
- Verified the changes through the API and frontend.

## What I Chose Not to Change

I did not modify the existing UI design, API structure, database schema, or unrelated components because they were not causing high-value issues found during the review. I kept the patch focused and avoided unnecessary changes.

## Biggest Remaining Risk

The project has limited automated test coverage. More tests would be useful for search/filter combinations, pagination edge cases, invalid parameters, and future changes.

## Tools / AI

I used VS Code, Maven, the browser, API testing, and Git. I used ChatGPT to help review the code, identify possible root causes, and structure the debugging process. I manually applied and verified the changes.