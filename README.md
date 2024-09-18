age = int(input("Enter the age:\n"))
print(f"Age of Dhoni is {age}")






question = input("Banerjee's Question:\n")
reply = "I will if I get a chance."
print(f"Dhoni's Reply:\n{reply}")
print(f"For Banerjee's question \"{question}\" Dhoni's confident reply was \"{reply}\".")





print("Team 1:")
team1_name = input("Team Name:\n")
team1_score = input("Score:\n")
team1_overs = input("Overs played:\n")
print("Team 2:")
team2_name = input("Team name:\n")
team2_score = input("Score:\n")
team2_overs = input("Overs played:\n")
print("Match Details:")
print(f"Team 1:\nName: {team1_name}\nScore: {team1_score}\nOvers played: {team1_overs}")
print(f"Team 2:\nName: {team2_name}\nScore: {team2_score}\nOvers played: {team2_overs}")



dhoni_age = int(input())
devki_age = (4 * (dhoni_age + 3)) - 3
print(devki_age)





X = int(input())
Y = int(input())
Z = float(input())
days = 30
total_distance = 2 * X * days
litres_needed = total_distance / Y
total_cost = litres_needed * Z
print(f"{total_cost:.2f}")




salary = int(input())
bonuses_awards = int(input())
endorsements = int(input())
total_income = salary + bonuses_awards + endorsements
salary_percentage = (salary / total_income) * 100
bonuses_awards_percentage = (bonuses_awards / total_income) * 100
endorsements_percentage = (endorsements / total_income) * 100
print(f"{salary_percentage:.2f} {bonuses_awards_percentage:.2f} {endorsements_percentage:.2f}")





no_balls = int(input())
wides = int(input())
byes = int(input())
leg_byes = int(input())
penalty_runs = int(input())
total_extras = (no_balls + wides + byes + leg_byes + (penalty_runs * 5))
print(total_extras)




X = int(input())
Y = int(input())
senior_players_count = 6
junior_players_count = 5
senior_contribution_rate = 0.50  # 50%
junior_contribution_rate = 0.40    # 40%
senior_contribution = senior_players_count * (X * senior_contribution_rate)
junior_contribution = junior_players_count * (Y * junior_contribution_rate)
total_contribution = senior_contribution + junior_contribution
print(f"{total_contribution:.2f}")







total_age = int(input())
a = (total_age - 10) / 3
age_x = int(a)
age_y = int(a)
age_z = age_x + 10
print(age_x)
print(age_y)
print(age_z)






x1 = int(input())
y1 = int(input())
x2 = int(input())
y2 = int(input())
mid_x = (x1 + x2) / 2
mid_y = (y1 + y2) / 2
print(f"Binoy's house is located at ({mid_x:.1f},{mid_y:.1f})")



import math
def calculate_distance(x1, y1, x2, y2):
    distance = math.sqrt((x2 - x1) ** 2 + (y2 - y1) ** 2)
    return distance
x1 = int(input("Enter x1: "))
y1 = int(input("Enter y1: "))
x2 = int(input("Enter x2: "))
y2 = int(input("Enter y2: "))
distance = calculate_distance(x1, y1, x2, y2)
print(f"Distance: {distance:.2f}")











x1 = int(input())
y1 = int(input())
x2 = int(input())
y2 = int(input())
x3 = int(input())
y3 = int(input())
area = 0.5 * abs(x1 * (y2 - y3) + x2 * (y3 - y1) + x3 * (y1 - y2))
print(f"{area:.2f}")


def calculate_slope(x1, y1, x2, y2):
    # Check for vertical line to avoid division by zero
    if x2 - x1 == 0:
        return "undefined"  # Slope is undefined for vertical lines
    slope = (y2 - y1) / (x2 - x1)
    return slope
x1 = int(input("Enter x1: "))
y1 = int(input("Enter y1: "))
x2 = int(input("Enter x2: "))
y2 = int(input("Enter y2: "))
slope = calculate_slope(x1, y1, x2, y2)
if slope == "undefined":
    print("Slope is undefined (vertical line).")
else:
    print(f"Slope: {slope:.2f}")


                                    Decision Making
x = int(input("Enter the first number (x): "))
y = int(input("Enter the second number (y): "))
if x == y:
    print("x and y are equal")
elif x > y:
    print("x greater than y")
else:
    print("x less than y")


def check_character(char):
    vowels = 'aeiouAEIOU'
     if char.isalpha():
        if char in vowels:
            return "Vowel"
        else:
            return "Consonant"
    else:
        return "Not an alphabet"
character = input("Enter a character: ")
if len(character) == 1:
    result = check_character(character)
    print(result)
else:
    print("Please enter a single character.")





def determine_grade(marks):
    if marks > 100:
        return "Invalid Input"
    elif marks == 100:
        return "S"
    elif 90 <= marks < 100:
        return "A"
    elif 80 <= marks < 90:
        return "B"
    elif 70 <= marks < 80:
        return "C"
    elif 60 <= marks < 70:
        return "D"
    elif 50 <= marks < 60:
        return "E"
    else:
        return "F"
marks = int(input("Enter the marks scored by the student: "))
grade = determine_grade(marks)
print(grade)





def calculate_profit_or_loss(total_cost, selling_price_per_banana):
    cost_per_banana = total_cost / 12
    total_selling_price = selling_price_per_banana * 12
    profit_or_loss = total_selling_price - total_cost

    return profit_or_loss
total_cost = float(input("Enter the total cost (X) for a dozen bananas: "))
selling_price_per_banana = float(input("Enter the selling price (Y) for one banana: "))
result = calculate_profit_or_loss(total_cost, selling_price_per_banana)
if result > 0:
    print(f"Profit: Rs. {result:.2f}")
elif result < 0:
    print(f"Loss: Rs. {abs(result):.2f}")
else:
    print("No Profit No Loss")






def calculate_fee(student_type, tuition_fee, additional_fee):
    if student_type == "MSDS":  
        total_fee = tuition_fee + additional_fee  # Bus fee
    elif student_type == "MSH": 
        total_fee = tuition_fee + additional_fee  # Hostel fee
    elif student_type == "MGSDS":  
        total_fee = 1.5 * tuition_fee + additional_fee  # Bus fee
    elif student_type == "MGSH": 
        total_fee = 1.5 * tuition_fee + additional_fee  # Hostel fee
    else:
        return None
    
    return total_fee
student_type = input("Enter the student type (MSDS, MSH, MGSDS, MGSH): ")
tuition_fee = float(input("Enter the tuition fee: "))
additional_fee = float(input("Enter the bus/hostel fee: "))
total_fee = calculate_fee(student_type, tuition_fee, additional_fee)
if total_fee is not None:
    print(f"Total Fee Amount: Rs. {total_fee:.2f}")
else:
    print("Invalid student type.")





birth_year = int(input("Enter your birth year (last two digits, e.g., '62'): "))
current_year = int(input("Enter the current year (last two digits, e.g., '99'): "))
age = current_year - birth_year
if age < 0:
    age += 100
print(f"Your current age is: {age} years")







a = int(input("Enter the seating capacity of Lab L1: "))
b = int(input("Enter the seating capacity of Lab L2: "))
c = int(input("Enter the seating capacity of Lab L3: "))
min_capacity = min(a, b, c)
print(f"The lab with the minimal seating capacity has: {min_capacity} seats")






a = int(input("Enter the seating capacity of Lab L1: "))
b = int(input("Enter the seating capacity of Lab L2: "))
c = int(input("Enter the seating capacity of Lab L3: "))
allocated_lab = input("Enter the lab allocated for ACE training (L1, L2, L3): ").strip().upper()
labs = {
    "L1": a,
    "L2": b,
    "L3": c
}
if allocated_lab in labs:
    del labs[allocated_lab]
min_lab = min(labs, key=labs.get)
min_capacity = labs[min_lab]
print(f"The lab with the minimal seating capacity among the available labs is {min_lab} with {min_capacity} seats.")





a = int(input("Enter the seating capacity of Lab L1: "))
b = int(input("Enter the seating capacity of Lab L2: "))
c = int(input("Enter the seating capacity of Lab L3: "))
n = int(input("Enter the number of students: "))
accommodating_labs = 0
if a >= n:
    accommodating_labs += 1
if b >= n:
    accommodating_labs += 1
if c >= n:
    accommodating_labs += 1
print(f"Number of labs that can accommodate {n} students: {accommodating_labs}")





x = int(input("Enter the seating capacity of Lab L1: "))
y = int(input("Enter the seating capacity of Lab L2: "))
z = int(input("Enter the seating capacity of Lab L3: "))
n = int(input("Enter the number of students: "))
best_lab = None
max_capacity = -1
if x >= n and x > max_capacity:
    max_capacity = x
    best_lab = "L1"
if y >= n and y > max_capacity:
    max_capacity = y
    best_lab = "L2"
if z >= n and z > max_capacity:
    max_capacity = z
    best_lab = "L3"
if best_lab:
    print(f"The suitable lab for {n} students is: {best_lab}")
else:
    print("No lab can accommodate the specified number of students.")

































