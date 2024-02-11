# Lab Report 3: Bugs and Commands
## Part 1: Bugs 

Choose one of the bugs from week 4's lab.

Provide:

- A failure-inducing input for the buggy program, as a JUnit test and any associated code (write it as a code block in Markdown)
- An input that doesn't induce a failure, as a JUnit test and any associated code (write it as a code block in Markdown)
- The symptom, as the output of running the tests (provide it as a screenshot of running JUnit with at least the two inputs above)
- The bug, as the before-and-after code change required to fix it (as two code blocks in Markdown)
Briefly describe why the fix addresses the issue.



**Failure-Inducing Input**:
```
  @Test
  public void testReversedEvenLength() {
    int[] input2 = { 1,2 };
    assertArrayEquals(new int[]{ 2,1 }, ArrayExamples.reversed(input2));
  }
```
**Non-Failure-Inducing Input**:
```
  @Test
  public void testReversedEmptyArray() {
    int[] input1 = { };
    assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
  }
```
**Symptom**:
![Image]() ![Image]() \
**Bug**:

Before:
```
  static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
```
After:
```
  static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }
```
Explanation: Before, the value of each index in the new, empty array was assigned to the indices of the original array, making all of the values zero. Simply switching the assignment by putting the original array values into the new array with the values' new positions will make the new array contain the reversed array. The last thing to fix is to then return the new, reversed array rather than the original array.

## Part 2: Researching Commands
**Command [ ]**
Option 1:
* Example 1
* Example 2
Option 2:
* Example 1
* Example 2
Option 3:
* Example 1
* Example 2
Option 4:
* Example 1
* Example 2
