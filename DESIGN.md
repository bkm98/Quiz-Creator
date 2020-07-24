# Design

## Description
Quiz Creator is a system that allows users (students and educators), to make, take, save
(either to their local machine or a database, which will come in a later iteration), and edit
quizzes for the purpose of studying and refining their knowledge. The user interface is designed
in such a way that makes it easy to learn and simple to use, without losing any of its
required functionality. 

## Architecture

## Class Diagram

## Sequence Diagram

	-User Case: Taking a local quiz
	Actor: User
	Description: The user can take a local quiz once it has been created
	Pre-Conditions: The user has already created a local quiz and saved it to their local drive
	Post-Conditions: The quiz has been taken and have fed back a grade
	Main Flow & Alternative Flows (shown with #.# format):
		1. User enters a Quiz Title into a search box
		2. System finds local quiz and displays the quiz taker screen
			2.1. System is unable to find a quiz with matching quiz title
			2.2. System informs the user that the quiz title entered does not exist and that the
				 quiz was not found.
			2.3. System prompts the user to try searching for another quiz title.
		3. User goes through quiz questions and answers accordingly.
		4. System receieves responses and saves them.
		5. User submits quiz once finished.
		6. System compares user responses to answers declared by quiz creator.
		7. System displays quiz results back to user.

## Design Patterns

## Design Principles
	SOLID Principles
	-Single responsibility principle
		-A class should only have 1 responsibility
	-Open/Closed principle
		-Entities should be open for extension but closed for modification
	-Liskov substitution principle
		-Objects in a program should be able to be replaced with instances of their subtypes without altering correctness of the program
	-Interface segregation principle
		-Many client-specific interfaces are better than one general-purpose interface
	-Dependency inversion principle
		-Depend upon abstractions, not concretions