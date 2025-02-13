# MongoDB $inc Operator with String Value
This repository demonstrates an uncommon bug in MongoDB related to the incorrect usage of the `$inc` operator.  The `$inc` operator is designed to increment a numerical field by a specified value.  However, using a string instead of a number can lead to unexpected behavior and data corruption.  This example highlights this error and demonstrates the correct usage of `$inc`.

## Bug
The primary issue is the use of a string ('1') instead of a number (1) with the `$inc` operator.  This results in the `count` field not being incremented correctly.