## Lab 4: Child Vaccination Chart ##

```python
## below is a function "insert" that asks for first name, last name, and birthdate
patient = {}
vac_types = ['HepB', 'RV', 'DTaP', 'Hib', 'PCV13', 'IPV', 'IIV4', 'MMR', 'VAR', 'HepA']

def insert():
    vac_month = {}

    patient_id = input("Please enter the patient record number: ")
    f_name = input("What is the first name? ")
    l_name = input("What is the last name? ")

    for key in vac_types:
        answer = input(f"What month did patient receive the {key} vaccine? ")
        vac_month[key] = answer

    patient_details = {'first': f_name, 'last': l_name, 'vaccines': vac_month}
    patient[patient_id] = patient_details

    for x, y in patient.items():
        print(f"{x} : {y}")

insert()
while True:
        choice = input("Would like to enter another patient record (y/n)? ")
        if choice == "yes" or "y":
            insert()
        elif choice == "no" or "n":
            print("Closing program...have a nice day!")
        else:
            print("Please type 'y' or 'n'")
```

