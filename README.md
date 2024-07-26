# Welcome message
print("Welcome to Python Pizza Deliveries!")

# Get user input for pizza size
size = input("What size pizza do you want? (S, M, L): ")

# Get user input for pepperoni
add_pepperoni = input("Do you want pepperoni? (Y/N): ")

# Get user input for extra cheese
extra_cheese = input("Do you want extra cheese? (Y/N): ")

# Calculate the base price based on pizza size
if size == "S":
    base_price = 15
elif size == "M":
    base_price = 20
else:
    base_price = 25

# Add pepperoni cost
if add_pepperoni == "Y":
    if size == "S" or size == "M":
        base_price += 2
    else:
        base_price += 3

# Add extra cheese cost
if extra_cheese == "Y":
    base_price += 1

# Display the final bill
print(f"Your final bill is: ${base_price}.")
