import tkinter as tk
from datetime import datetime, timedelta

def calculate_due_date():
    # Get the input from the Date Entry field
    lmp_str = date_entry.get()

    try:
        # Convert the input string to a datetime object
        lmp = datetime.strptime(lmp_str, "%Y-%m-%d")

        # Calculate the due date by adding 280 days to the LMP
        due_date = lmp + timedelta(days=280)

        # Update the result label in the GUI
        result_label.config(text="Your due date is: {}".format(due_date.strftime("%Y-%m-%d")))

    except ValueError:
        # Display error message in the GUI
        result_label.config(text="Invalid date format. Please enter in YYYY-MM-DD format.")

# Create the main window
window = tk.Tk()
window.title("Due Date Calculator")

# Create a label and entry field for the LMP input
date_label = tk.Label(window, text="Date of Last Menstrual Period (YYYY-MM-DD):")
date_label.pack()
date_entry = tk.Entry(window)
date_entry.pack()

# Create a button to calculate the due date
calculate_button = tk.Button(window, text="Calculate", command=calculate_due_date)
calculate_button.pack()

# Create a label to display the due date result
result_label = tk.Label(window, text="")
result_label.pack()

# Start the GUI event loop
window.mainloop()
