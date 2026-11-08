#The purpose of this program is to calculate the total number of chairs in a classroom environment
rows = 6
chairs_per_row = 8
total_chairs = rows * chairs_per_row

print("Number of rows:", rows)
print("chairs per row:" , chairs_per_row)
print("Total number of chairs:", total_chairs)

#Student Weekly Expense Calculator
print("=" * 38)
print("SYUDENT EXPENSE TRACKER")
print("WEEKLY EXPENSE REPORT")
print("=" * 38)

 #INPUT CODE
student_name = input("Enter student name: ")
daily_transport_cost = float(input("Enter daily transport cost(NGN): "))
daily_feeding_cost = float(input("Enter daily feeding cost (NGN): "))
days_on_campus = int(input("Enter number of days on campus: "))
other_weekly_expenses = float(input("Enter other expenses during the week: "))

                     #PROCESS CODE
transport_total = daily_transport_cost * days_on_campus
feeding_total = daily_feeding_cost * days_on_campus
weekly_total = transport_total + feeding_total + other_weekly_expenses

                     #OUTPUT CODE
print("\n" + "=" * 38)
print("WEEKLY EXPENSES")
print("=" * 38)
print(f"Student: {student_name}")
print("-" * 38)
print(f"Transport Total: NGN {transport_total:,.2f}")
print(f"Other Expenses: NGN {other_weekly_expenses:,.2f}")
print("-" * 38)
print(f"Weekly Total: NGN {weekly_total:,.2f}")
print("=" * 38)
print("Done using Student Expense Tracker")
                     




#MULTIPLICATION TABLE
while True:
    print("\nMULTIPLICATION TABLE")
    print("Enter e to exit")


    user_input = input("Enter a whole number greater than 1: ")

    if user_input.lower() == "e":
        print("Program terminated.")
        break

    try:
        number = int(user_input)

        if number <= 1:
            print("Invalid input! Number must be greater than 1.")
            continue

        for i in range(1, 13):
            print(number, "x", i, "=", number * i)

    except ValueError:
        print("Invalid input! Enter a whole number or E to exit.")
        
