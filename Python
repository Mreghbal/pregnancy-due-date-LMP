def calculate_due_date(lmp):
    # Calculate the due date by adding 280 days to the LMP
    due_date = lmp + timedelta(days=280)
    return due_date

# Get input from the user
lmp_str = input("Enter the date of your last menstrual period (YYYY-MM-DD): ")

# Convert the input string to a datetime object
lmp = datetime.strptime(lmp_str, "%Y-%m-%d")

# Calculate the due date
due_date = calculate_due_date(lmp)

# Print the due date
print("Your due date is:", due_date.strftime("%Y-%m-%d"))
