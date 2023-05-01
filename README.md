Download Link: https://assignmentchef.com/product/solved-bits-and-pieces-part-1
<br>
<strong><u>Objective</u></strong>: With the introduction of different numeral systems and insight into how to convert from one to the other, and vice-versa, you will now gain some firsthand experience on how to define functions that work with binary and decimal numbers. To be able to differentiate between binary and decimal numbers, on top of being able to work with them, binary numbers will be represented as strings with decimal numbers represented as they are. This will be useful for many reasons. The first is that, when creating a function that deals with binary numbers, it will expect a string. If it receives anything other than a string, there may be another portion of code that will notify the user if this is the case. This is known as exception handling, but this assignment will not be covering it.




<h2>Required Functions</h2>




<h3>            is_binary(string)</h3>

<em>                         </em>

<em>                                    </em><strong>Description</strong>: Determine if the passed string meets the necessary criteria for it to  be a binary number.




<strong>Output</strong>: This function should not print anything onto the screen.




<strong>Return Value</strong>: Return <strong>False</strong> if the given string is not in the correct binary number format. Return <strong>True</strong> otherwise.




<h3>binary_to_decimal(binary_string)</h3>

<em> </em>

<strong>Description</strong>: Convert the given binary number to a decimal number. During testing, a non-binary number may be passed as an argument. Ensure that you handle this case as appropriate.




<strong>Output</strong>: This function should not print anything onto the screen.




<strong>Return Value</strong>: If the passed string is valid, return an integer representing the decimal value of the binary number. Otherwise, return -1.




<strong>Suggestions</strong>: Recall that each bit has a weight to it that is based on its position in the sequence of numbers. For example, in the binary number 1100<sub>b</sub>, the weight

of the third bit is 2<sup>2</sup>. This may be difficult to implement in practice, but there is a

method in computer science known as Horner’s Method

<a href="https://en.wikipedia.org/wiki/Horner's_method#Application">(</a><a href="https://en.wikipedia.org/wiki/Horner's_method#Application">https://en.wikipedia.org/wiki/Horner’s_method#Application</a><a href="https://en.wikipedia.org/wiki/Horner's_method#Application">)</a> that employs a very practical formula in obtaining the resulting decimal value of the binary number, and it is as follows:

<strong>             </strong>

baseTen = baseTen * 2 + bit[i],




with i representing the position of the bit.







<h3>            decimal_to_binary(deci)</h3>




<strong>Description</strong>: Convert the passed decimal number <em>deci</em> to a binary format.




<strong>Output</strong>: This function should not print anything onto the screen.




<strong>Return Value</strong>: A string that is the binary representation of the decimal number.




<strong>Suggestions</strong>: The algorithm in converting from decimal to binary can be implemented here. In regards to storing the obtained bit at each step, using a list is advisable but not required. Do recall that the bits are obtained in an “opposite” ordering, meaning that the first bit obtained will actually be the last bit in the sequence, and vice-versa. A big hint to approaching this is first creating an empty list, and an empty string. When implementing the algorithm, append each obtained bit to the end of the list. Once obtaining all bits, utilize string concatenation to include each bit in the string sequence, then return that string.







<h3>bitwise_add(binary_string1, binary_string2)</h3>

<em> </em>

<strong>Description</strong>: Add two binary numbers to obtain the result of the addition. During testing, one or both passed strings may not be valid binary numbers. Ensure that you handle this case as appropriate.




<strong>Output</strong>: This function should not print anything onto the screen.




<strong>Return Value: </strong>A string representing the binary number that is the sum of the two passed binary numbers. If one or both passed strings are not valid, return the string “Error”.




<strong>Suggestions</strong>: You may use the previous two functions, <strong>binary_to_decimal() </strong>and <strong>decimal_to_binary</strong>() to implement this function.







<h2>Testing</h2>




Total tests: 22




<strong>is_binary()</strong> will have 4 test cases. All other functions will have 6 test cases.




<h2> Notes</h2>




Name your program “bits_and_pieces.py”, otherwise the program tester will NOT work.





