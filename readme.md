Medical Diagnostic Expert System (Prolog)
Overview
This project is a Medical Diagnostic Expert System developed in Prolog.
It interacts with the user by asking a series of symptom-based questions and attempts to diagnose a possible illness based on the responses.

Features
Interactive command-line interface
Rule-based disease diagnosis
Supports multiple illnesses:
COVID-19
Influenza
Common Cold
Allergies
Dynamic knowledge base using Prolog facts
Backtracking control using cut (!) operator
 How It Works
1.	The system starts by displaying a welcome message.
2.	It asks the user a series of yes/no questions about symptoms.
3.	Based on responses, it matches symptoms with predefined rules.
4.	Once a match is found, it outputs the diagnosis.
5.	If no match is found, it returns unknown_illness.

Usage Instructions
 Run the Program
1.	Open your Prolog environment (e.g., SWI-Prolog).
2.	Load the file:
3.	[filename].
4.	Start the system:
5.	start.

Answer Format
	Type:
	y. for Yes
	n. for No
	Disease Rules
Disease	Required Symptoms
COVID-19	fever, dry_cough, loss_of_taste_or_smell
Influenza	fever, headache, body_ache, chills
Common Cold	sneezing, runny_nose, sore_throat
Allergies	sneezing, watery_eyes, itchy_nose

Key Predicates
start/0
	Entry point of the program
	Displays instructions and begins diagnosis
diagnose/1
	Determines the disease using hypothesis rules
hypothesis/1
	Contains rules for each disease
verify/1
	Checks if a symptom is already known or asks the user
ask/1
	Prompts the user for input
undo/0
	Clears stored facts after diagnosis

Example Interaction
Do you have this symptom - fever? (y./n.): y.
Do you have this symptom - dry_cough? (y./n.): y.
Do you have this symptom - loss_of_taste_or_smell? (y./n.): y.

DIAGNOSIS RESULT: covid_19

Disclaimer
This system is built for educational purposes only.
It does not provide real medical diagnosis. Always consult a qualified healthcare professional for medical concerns.

Future Improvements
	Add more diseases and symptoms
	Improve user interface
	Integrate probabilistic reasoning
	Add GUI support

Author
Developed as part of an AI/Prolog academic project.

