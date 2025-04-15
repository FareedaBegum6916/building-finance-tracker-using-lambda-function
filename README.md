# building-finance-tracker-using-lambda-function
📚 What I Learned – Scientific Computing with Python (freeCodeCamp)
As part of my Scientific Computing with Python certification from freeCodeCamp, I built a terminal-based Expense Tracker application using core Python programming concepts. Through this project, I practiced and applied fundamental and intermediate concepts that are essential to scientific computing and real-world problem-solving.

🧱 Data Structures
I used lists and dictionaries to store and manage expenses in a structured way. Each expense was stored as a dictionary with amount and category keys, and all such entries were maintained in a list. This helped me understand how to organize data efficiently and retrieve it later for filtering or calculations.

python
Copy
Edit
expenses.append({'amount': amount, 'category': category})
🧮 Functional Programming Tools: map(), filter(), lambda
One of the major highlights of this project was using Python’s functional programming tools:

map() was used in the total_expenses() function to extract the amount field from each expense and then pass the result to sum() to get the total spending.

python
Copy
Edit
return sum(map(lambda expense: expense['amount'], expenses))
filter() was used in the filter_expenses_by_category() function to return only those expenses that matched the user-provided category.

python
Copy
Edit
return filter(lambda expense: expense['category'] == category, expenses)
lambda functions made the code more concise by allowing me to write one-line anonymous functions, which are especially useful when used with map() and filter().

🔄 Control Flow & User Interaction
I created an infinite while loop to keep the program running until the user chooses to exit. Inside this loop, I used if-elif-else statements to respond to user choices and execute different functionalities such as adding a new expense, viewing all expenses, or filtering by category. The loop is broken using the break statement when the user selects the "Exit" option.

python
Copy
Edit
while True:
    # menu options
    if choice == '5':
        break
💡 Modular Programming
I split the logic into reusable functions to keep the code modular and clean. Each function performed a single responsibility (like adding an expense or filtering the list), which made the program easier to read, test, and maintain.

📌 Summary
Overall, this project helped me gain hands-on experience with data handling, functional programming (lambda, map(), filter()), user input, loops, conditionals, and modular code design. It brought together several key Python concepts that I learned during the Scientific Computing with Python curriculum and gave me the confidence to build interactive CLI tools that reflect real-world use cases.
