# CSE 15L WI 23 Lab Report 2

## 1.

## 2. Bugs
Code:
'''
static double averageWithoutLowest(double[] arr) {
  if(arr.length < 2) { return 0.0; }
    double lowest = arr[0];
    for(double num: arr) {
      if(num < lowest) { lowest = num; }
    }
    double sum = 0;
    for(double num: arr) {
      if(num != lowest) { sum += num; }
    }
    return sum / (arr.length - 1);
}
'''
Test:
```
private static final double DELTA = 1e-15;

 @Test
 public void newAverageWithoutLowest() {
   double[] arr = {1.0, 1.0, 3.5, 5.0, 3.5};
   double[] arr2 = {2.5, 1.5, 6.0, 3.5};
   assertEquals(3.25, ArrayExamples.averageWithoutLowest(arr), DELTA);
   assertEquals(4.0, ArrayExamples.averageWithoutLowest(arr2), DELTA);
 }
```
The test above would provide the following output:
# insert image

A symptom from the code above would be shown when there was two numbers that were equal to one another that where it was also the lowest number then 
instead of only exluding one of the numbers, the program would exlode both numbers. This is shown in the first test where it would result in the test 
failing because the program would output the double 3.0 instead of 3.25.



## 3.
