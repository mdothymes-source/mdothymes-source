## Lab 4: Child Vaccination Chart ##

```python
##creating an empty dictionary to fill with patient date
patient = {}
##i created a list with all the different vaccines that will be referenced later
vac_types = ['HepB', 'RV', 'DTaP', 'Hib', 'PCV13', 'IPV', 'IIV4', 'MMR', 'VAR', 'HepA']

## below is a function "insert" that asks for first name, last name, and birthdate
def insert():
    vac_month = {} ##empty dictionary for the nested dictionary that will hold all the vaccine data

    ##invoking user input for patient data
    patient_id = input("Please enter the patient record number: ")
    f_name = input("What is the first name? ")
    l_name = input("What is the last name? ")

    ##i made a for loop to iterate through the list of vac_types and asks about each vaccine individually
    ##then i use the answers and the same vac_type list to make a key-value pair to go inside the patient_details dictionary 
    for key in vac_types:
        answer = input(f"What month did patient receive the {key} vaccine? ")
        vac_month[key] = answer

    patient_details = {'first': f_name, 'last': l_name, 'vaccines': vac_month}
    patient[patient_id] = patient_details

    ##i made a loop for the print statement to have it print one record for each line
    for x, y in patient.items():
        print(f"{x} : {y}")

insert() ##calling the function i made to ask for user input
##this while true loop is used to ask the user if they want to continue entering patient data or quit the program
while True:
        choice = input("Would like to enter another patient record (y/n)? ")
        if choice == "yes" or "y":
            insert()
        elif choice == "no" or "n":
            print("Closing program...have a nice day!")
        else:
            print("Please type 'y' or 'n'")
```

