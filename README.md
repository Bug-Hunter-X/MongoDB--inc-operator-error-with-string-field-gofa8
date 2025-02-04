# MongoDB $inc operator error with string field
This repository demonstrates a common error when using the `$inc` operator in MongoDB. The `$inc` operator is used to increment a numerical field by a specified value. However, attempting to use it on a field that is not of a numeric type will result in an error.

## Bug
The bug occurs when using the `$inc` operator with a field that is of string type.  The MongoDB driver will throw an error in this case.

## Solution
The solution involves ensuring that the field being incremented is of a numeric type (e.g., NumberInt, NumberLong, NumberDecimal). You might need to modify the data in your collection, or change how the data is stored initially.
