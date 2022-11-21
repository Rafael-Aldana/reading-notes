# Operators and Loops

The importance of operators and loops in this class is pretty important because we'll be using them a lot throughout the course.

This part of class we're looking into expressions and operators. An expression is a valid unit of code that resolves to a value. There are two types of expressions: those that have side effects(such as assigning values) and those that purely evaluate. ex: x=7 this expression uses the = operator to assign the value seven to the variable x. The expression itself evaluates to 7 (mdn web docs).
An assignment operator is an operator that assigns a value to its left operand based on the value of its right operand.
ex: x = f()
    x is the left operand = is the operator and f() is the right operand. That is, x = f() is an assignment expression that assigns the value of f() to x.
A comparison operator is an operator that compares its operands and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values. Strings are compared based on standard lexicographical ordering, using unicode values. Most of the time JS tries to change the operands to an appropriate type for the comparison if the two opperands are not of the same type.

## Things that I want to know more about

The operators AND/OR have almost the same look to them in my eyes, but for AND operators if one is not true the whole expression is false. As oppose to OR if one is not true the entire expression doesn't automatically become false.