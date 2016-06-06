# The while loop
The while loop is generally preferred if the number of times we need to loop is not fixed. It is widely used in event-driven-programming where the number of loop iterations is decided by user events.
Here is a simple program to print an even number as long as user does not press 'q' key.
```
start_number = 0
current_number = start_number
while(True):
  print(current_number)
  user_input = input('enter q to quit')
  if user_input == 'q':
    break
  current_number += 2
```
* input( ) -reads user input, returns user input as string
* break - used to abruptly jump out of current enclosing loop

The syntax for a while loop is
```
while expression:
  statement
  ```
Here value of the expression decides whether the loop body can be entered or not.

