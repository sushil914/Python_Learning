import math

def Calculater_Function(label):
    count = int(input(f"How many values for {label}?\n"))
    return sum(
        int(input(f"Enter number {i + 1}: "))
        for i in range(count)
    )       


first_total = Calculater_Function("First Input")
second_total = Calculater_Function("Second Input")

addition = first_total + second_total
subtraction = first_total - second_total
multiplication = first_total * second_total
division = first_total / second_total if second_total != 0 else "Undefined (division by zero)"

print(f"\nTotal Addition       : {addition}")
print(f"Total Subtraction    : {subtraction}")
print(f"Total Multiplication : {multiplication}")
print(f"Total Division       : {division}")
