# MongoDB $inc Operator Error

This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations. The `$inc` operator is used to increment or decrement a numerical field by a given value.  However, the value provided must be a number; providing a string will result in an error.

## Bug
The original code incorrectly passes a string ('1') to the `$inc` operator.  This causes the update operation to fail.

## Solution
The corrected code uses a numeric value (1) for the increment, ensuring the operation succeeds.