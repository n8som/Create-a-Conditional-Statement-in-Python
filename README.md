# Create-a-Conditional-Statement-in-Python

<h2>Introduction</h2>

Conditional statements are a powerful structure that helps in achieving automation when I need to make sure conditions are met before certain actions are executed. For example, security analysts can use conditional statements in Python to check if users are approved to access a device.

In this lab, I will practice writing conditional statements in Python.

<h2>Scenario</h2>

I'm working as a security analyst. First, I am responsible for checking whether a user's operating system requires an update. Then, I need to investigate login attempts to a specific device. I must determine if login attempts were made by users approved to access this device and if the login attempts occurred during organization hours.

<h2>Task 1</h2>

I am asked to help automate the process of checking whether a user's operating system requires an update. Imagine that a user's device can be running one of the following operating systems: OS 1, OS 2, or OS 3. While OS 2 is up-to-date, OS 1 and OS 3 are not. My task is to check whether the user's system is up-to-date, and if it is, display a message accordingly. To do this, complete the conditional statement using the keyword if.

<h2>Task 2</h2>

Now try assigning the system variable to different values ("OS 1", "OS 2", and "OS 3"), run the cell, and observe what happens. Keep the conditional statement as is.

Question 1

What happens when OS 2 is running? What happens when OS 1 is running?

<h2>Task 3</h2>

Nothing is displayed when the system is not equal to "OS 2". This is because the condition didn't evaluate to True.

It would be beneficial if an alternative message is provided to them when updates are needed.

In the following cell, add the appropriate keyword after the first conditional so that it will display a message that conveys that an update is needed when the system is not running OS 2. 

Then, set the value of the system variable to indicate that OS 2 is running and run the cell. After observing what happens, set the value of system to indicate either that OS 1 is running or that OS 3 is running and run the cell.

Question 2

In this setup what happens when OS 2 is running? And what happens when OS 2 is not running?

[Double-click to enter Ir responses here.]

<h2Task 4</h2>

This setup is still not ideal. If the variable system contains a random string or integer, the conditional above would still display update needed.

To improve the conditional, I will need to add the elif keyword. In the following cell, I will add two elif statements after the if statement, to create the final code. The first elif statement will display update needed if system is "OS 1". The second elif statement will display the same message, if system is "OS 3". Complete the second elif statement, and then run the cell with the variable system set to a different string each time. Observe what happens when each operating system is running. Also try assigning the system variable to some strings other than "OS 1", "OS 2", and "OS 3" (for example "OS 4").

Question 3

Under this setup what happens when OS 2 is running? What happens when OS 1 is running? What happens when OS 3 is running? What happens when neither of those three operating systems are running?

<h2>Task 5</h2>

Writing code that is readable and concise is best practice in programming.

The conditional above can be written more concisely.

In the following cell, use a logical operator to combine the two elif statements from the previous setup into one elif statement. 

Then, assign the system variable to a value and run the cell. Like I did in the previous task, use "OS 1", "OS 2", "OS 3", and other strings.

Question 4

What do I observe about this conditional?

<h2>Task 6</h2>

Now I'll move on to the next part of my work. I've been asked to investigate login attempts to a specific device. Only approved users should log on to this device.

I'll start with two authorized users, stored in the variables approved_user1 and approved_user2. I'll need to write a conditional statement that compares those variables to a third variable, username. This will be the username of a specific user trying to log in.

<h2>Task 7</h2>

The number of approved users has now expanded to five. Rather than storing each of the approved users' usernames individually, it would be more concise to store them in an allow list called approved_list.

The ```in``` operator in Python can be used to determine whether a given value is an element of a sequence. Using the in operator in a condition can help me check whether a specific username is part of a list of approved usernames. For example, in the code below, username in approved_list evaluates to True if the value of the username variable is included in approved_list.

Complete the code in the following cell to display the same messages that I used in the previous step. When the condition evaluates to True, the following message will be displayed: "This user has access to this device." When it evaluates to False, the following message will be displayed: "This user does not have access to this device." Then, run the cell to observe its behavior. Afterward, reassign the username variable to a username that is not approved and run the cell to observe what happens.

Question 5

What happens when an approved user tries to log in? What happens when an unapproved user tries to log in?

<h2>Task 8</h2>

Now I'll write another conditional statement. This one will use a organization_hours variable to check if the user logged in during specific organization hours. When that condition is met, the code should display the string "Login attempt made during organization hours.". When that condition isn't met, the code should display the string "Login attempt made outside of organization hours.".

The organization_hours variable will have a Boolean data type. If organization_hours has a Boolean value of True, that means the user is logged in during the specified organization hours. If organization_hours has a Boolean value of False, that means the user is not logged in during those hours.

Complete the conditional in the following cell.

Question 6

What happens when the user logs in during organization hours? What happens when they log in outside of organization hours?

<h2>Task 9</h2>

The following cell assembles the code from the previous tasks. It includes the conditional statement that checks if a user is on the allow list and the conditional statement that checks if the user logged in during organization hours.

Run the cell below a few times. Each time, enter a different combination of values for username and organization_hours to observe how that affects the output.

Question 7

What happens when the user trying to log in is not among the approved users? What happens when the user trying to log in is among the approved users? What happens when the user tries to log in outside of organization hours?

<h2>Task 10</h2>

I can also provide a single message about the login attempt. To do this, I can join both conditions into a single conditional statement using a logical operator. This will make the code more concise.

Examine the code in the following cell and add the missing operator that would allow for a single message. Then run the cell, entering different combinations of information, and observe what happens.

Question 8

In this setup, what happens when the user trying to log in is an approved user and doing so during organization hours? What happens when the user either is not approved or attempts to log in outside of organization hours?

<h2>Conclusion</h2>

What are the key takeaways from this lab?

- Conditional statements, comparison operators, and logical operators play a major role in automating important processes to maintain security, such as detecting when a user's operating system requires updates and detecting when a user is allowed to access a device.
- Conditional statements allow me to determine whether a specific set of conditions has been met.
- Comparison operators allow me to compare pairs of values. Specifically, the ```==``` operator allows me to determine whether one value is equal to another.
- Logical operators such as ```and``` and ```or``` allow me to check more than one condition at a time.

