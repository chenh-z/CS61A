## 1.2 Elements of Programming
#### 1.2.4 Names and the Environment
Changing the value of one name does not affect other names. Below, even though the name area was bound to a value defined originally in terms of radius, the value of area has not changed. Updating the value of area requires another assignment statement.

With multiple assignment, all expressions to the right of = are evaluated before any names to the left are bound to those values. As a result of this rule, swapping the values bound to two names can be performed in a single statement.

#### 1.2.6 The Non-Pure Print Function
The interactive Python interpreter does not automatically print the value None
