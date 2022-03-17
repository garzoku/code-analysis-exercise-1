# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident until you're confident that you know how the function works.
* Write a summary of what the function does.

```js
function (number){
  let table = ""

  const count = Array(10).fill(true)

  for (iteration in count) {
    let spacer = ""
    if (iteration < 10){
      spacer = "\n"
    }
    table = `${table}${iteration} * ${number} = ${iteration * number}${spacer}`
  }

  return table
}
```

| Input | Output        |
| ----- | ------------- |
|   1   | "1 * 1 = 1"   |
          "2 * 1 = 2"   |
          "3 * 1 = 3"   |
          "4 * 1 = 4"   |
          "5 * 1 = 5"   |
          "6 * 1 = 6"   |
          "7 * 1 = 7"   |
          "8 * 1 = 8"   |
          "9 * 1 = 9"   |
          "10 * 1 = 10" |
|   2   | "1 * 2 = 2"   |
          "2 * 2 = 4"   |
          "3 * 2 = 6"   |
          "4 * 2 = 8"   |
          "5 * 2 = 10"  |
          "6 * 2 = 12"  |
          "7 * 2 = 14"  |
          "8 * 2 = 16"  |
          "9 * 2 = 18"  |
          "10 * 2 = 20" |
|   3   | "1 * 3 = 3"   |
          "2 * 3 = 6"   |
          "3 * 3 = 9"   |
          "4 * 3 = 12"  |
          "5 * 3 = 15"  |
          "6 * 3 = 18"  |
          "7 * 3 = 21"  |
          "8 * 3 = 24"  |
          "9 * 3 = 18"  |
          "10 * 3 = 30" |

<table>
  <tr>
    <th>What does this program do?</th>
    <td>1). The function accepts a number as an input.
2). The table variable is declared as an empty string.<br>
3). The count variable is declared as an Array containing 10 values of true.<br>
4). A For loop cycles through each value in the array.<br>
5). For every iteration, the spacer variable is declared as an empty string.<br>
6). If the current iteration is less than 10 (if this iteration is not the last value in the array) the value of spacer is changed to a string of "\n"<br>
7). The table variable is assigned the appropriate string values, the iteration is multiplied by the number, and then a new line of table is created.<br>
8). The For loop continues to execute it's own code block until it iterates through every value in the array. Through each iteration, the table variable is assigned the equation's resulting value.<br>
Summary). This function will return a 10-row multiplication table for the entered number.</td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible
