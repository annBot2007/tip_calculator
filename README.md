# tip_calculator

# Project Goal: Create a tip calculator that calculates the tip according to the total bill,
# percentage tip desired, and number of people splitting the bill

print("-----------------------------------")
print("Welcome to the tip calculator!")
print("-----------------------------------")

total_amount = float(input("What was the total bill?: "))
tip_percentage = float(input("How much tip would you like to give? 10, 12, or 15?: "))
number_of_people = int(input("How many people to split the bill?: "))

total_tip = (tip_percentage / 100) * total_amount
tip_per_person = total_tip / number_of_people
amt_per_person = total_amount / number_of_people

total_amount_per_person = round(amt_per_person + tip_per_person, 2)

print(f"Each person should pay: ${total_amount_per_person} ")

