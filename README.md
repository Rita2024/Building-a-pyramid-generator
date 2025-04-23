# Character Pyramid Pattern Generator

## Description

This JavaScript code generates a symmetrical pattern of a specified character, resembling a pyramid or an inverted pyramid, in the console.

## How it works

The script uses the following variables:

* `character`:  The character used to build the pattern (default: "!").
* `count`: The number of rows in the pattern (default: 10).
* `rows`: An array to store each row of the pattern.
* `inverted`: A boolean to determine if the pyramid is inverted (default: false)

The script works as follows:

1.  **`padRow(rowNumber, rowCount)` Function**:
    * This function calculates the spaces and characters needed for each row.
    * It takes the row number and the total row count as input.
    * It returns a string with the correct number of leading spaces, characters, and trailing spaces to center the pattern.

2.  **Loop to Generate Rows**:
    * A `for` loop iterates from 1 to `count` (inclusive).
    * In each iteration, the `padRow()` function generates the string for that row.
    * If the `inverted` variable is false, the row is added to the end of the `rows` array.
    * If the `inverted` variable is true, the row is added to the beginning of the `rows` array.

3.  **Output the Pattern**:
    * The script iterates through the `rows` array.
    * Each row is appended to the `result` string, followed by a newline character ("\n").
    * Finally, the complete `result` string is printed to the console using `console.log()`.

## How to Use

1.  **Include in a JavaScript environment:** You can include this code in an HTML file using a `<script>` tag or run it in a Node.js environment.
2.  **Run the script:** The pattern will be printed to the console.

## Example Output

If `character` is "!" and `count` is 5, the output will be:

!
!!!!!!!!!!!!!!!!!!!!!!!!
If `character` is "!" , `count` is 5, and `inverted` is `true`, the output will be:

!!!!!!!!!!!!!!!!!!!!!!!!!
## Customization

You can modify the pattern by changing the following variables:

* `character`:  Change this string to use a different character in the pattern.
* `count`:  Change this number to control the height of the pattern.
* `inverted`: Set this boolean to `true` to create an inverted pattern.
