# Python_Day7
#Mini-Project: Calculate Power Dissipation of a Resistor
def calculate_power_dissipation(voltage, current):
    """
    Calculate the power dissipation of a resistor.
    
    Parameters:
    voltage (float): The voltage across the resistor in volts (V).
    current (float): The current through the resistor in amperes (A).
    
    Returns:
    float: The power dissipation in watts (W).
    """
    power = voltage * current
    return power

# Example usage:
try:
    voltage = float(input("Enter the voltage across the resistor (V): "))
    current = float(input("Enter the current through the resistor (A): "))
    power = calculate_power_dissipation(voltage, current)
    print(f"The power dissipation of the resistor is {power:.2f} watts.")
except ValueError:
    print("Invalid input. Please enter numerical values for voltage and current.")
