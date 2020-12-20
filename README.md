Small unit testing framework for Senegal.

![Passed](https://i.imgur.com/5D3hyvy.png)
![Failed](https://i.imgur.com/2zYr1A2.png)

## Example

```js
import 'modules/preen/src/preen.sgl'

function birbsAreAwesome() {
    testAssert(areBirbsAwesome());
}

test('birbsAreAwesome', birbsAreAwesome);
testsSummary();
```

## Usage
Within the root of your senegal project, run:

```sh
$ mkdir modules
$ git clone https://www.github.com/Calamity210/preen.git
```

Then import `modules/preen/src/preen.sgl` where needed.

## Functions
- testAssert(condition): Fails if condition is false.
- equal(left, right): Fails if left is not equal to right.
- notEqual(left, right): Fails if left is equal to right.
- diff(left, right, diff): Fails if the difference between left and right is greater than diff.
- isFalse(condition): Fails if condition is true.
- isTrue(condition): Fails if condition is false.
- isNotNull(object): Fails if object is null.
- isNull(object): Fails if object is null.
- test(name, function): Tests the passed function.
- testsSummary(): Returns a summary of tests.
- result(): Returns the results [testCount, failedTestsCount]

