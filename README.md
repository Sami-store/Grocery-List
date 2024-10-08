### Program Summary

This program allows a user to create a grocery list by prompting for the number of items, writing the list to a file, reading it back, and then displaying the list. The program is structured with the following methods:

1. **`getItemsArray(int numItems)`**:
   - Takes an integer parameter `numItems`.
   - If `numItems` is negative, it throws an exception.
   - Otherwise, it prompts the user to enter items in a loop for `numItems` iterations.
   - Returns an array of strings containing the entered items.

2. **`writeItems(String[] itemsArray, String fileName)`**:
   - Accepts an array of strings and a filename as parameters.
   - Writes the items from the array to a text file named according to the `fileName` parameter.
   - Catches any exceptions that may occur during the writing process.

3. **`readItems(String fileName)`**:
   - Takes a filename as a parameter and returns an `ArrayList` of strings.
   - Reads the contents of the specified file and populates the `ArrayList` with each line as an element.
   - Catches any exceptions that might occur during the reading process.

4. **`printList(ArrayList<String> itemsArrayList)`**:
   - Accepts an `ArrayList` of strings and prints each item on a separate line to the command line.

### Main Method Workflow

- Calls `getItemsArray` to obtain the grocery items based on user input.
- Passes the resulting array and a filename to the `writeItems` method to save the list.
- Calls `readItems` with the filename to retrieve the list into an `ArrayList`.
- Finally, passes the `ArrayList` to `printList` to display the items.

Throughout the execution, any exceptions that may arise are caught and handled appropriately.
