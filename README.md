# -Python-Project-14
#14 Simple Pizza Delivery 

print("Welcome to Python Pizza Deliveries!")
size = input("What size pizza do you want? (S,M or L)\n").capitalize()
add_pepperoni = input("Do you want pepperoni? (Y or N)\n").capitalize()
extra_cheese = input("Do you want extra cheese ? (Y or N)\n").capitalize()
bill = 0

if size == "S":
    bill += 15
elif size == "M":
    bill += 20
elif size == "L":
    bill += 25
else:
    quit()

if add_pepperoni == "Y":
    if size == "S":
        bill += 2
    else:
        bill += 3

if extra_cheese == "Y":
    bill += 1

print(f"The total for a Pizza ({size}) is ${bill}")
