# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers: missing error handling for invalid input.  Specifically, the provided code attempts to parse a user ID from the request parameters as an integer without verifying that it is indeed an integer. This can lead to unexpected behavior or crashes if the ID is not a valid number.

## Bug
The `bug.js` file contains the faulty code.  It attempts to find a user in the `users` array using the ID passed in the request parameters. However, it lacks error handling for non-numeric IDs, potentially causing a crash or incorrect results. 

## Solution
The `bugSolution.js` file shows how to correct the issue by adding proper error handling.  This includes validating the ID and returning appropriate error responses when necessary.