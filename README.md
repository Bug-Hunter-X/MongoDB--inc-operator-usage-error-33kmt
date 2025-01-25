# MongoDB $inc Operator Usage Error
This repository demonstrates a common error when using the `$inc` operator in MongoDB update queries.

## Problem
The `$inc` operator is used to increment a numerical field in a document.  However, incorrect usage can lead to unexpected behaviors or errors.
The example showcases incorrect usage where the key inside the `$inc` operator is not enclosed in double quotes within an object, leading to a query that doesn't update the document correctly. 
## Solution
The correct approach involves properly wrapping the field name within double quotes in an object, like `{"count":1}`.  This ensures the `$inc` operator correctly targets the specified field.