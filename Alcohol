import streamlit as st

def calculate_volume(unit, percentage):
    return (1000 * unit) / percentage

def calculate_percentage(volume, unit):
    return unit * (1000 / volume)

def calculate_unit(percentage, volume):
    return percentage / (1000 / volume)

def main():
    st.title("Unit-Volume-Percentage Calculator")

    choice = st.radio("Choose the value you want to calculate:", ["Volume", "Percentage", "Unit"])

    if choice == "Volume":
        unit_input = st.number_input("Enter unit:", min_value=0.0)
        percentage_input = st.number_input("Enter percentage:", min_value=0.0)
        result = calculate_volume(unit_input, percentage_input)

    elif choice == "Percentage":
        volume_input = st.number_input("Enter volume:", min_value=0.0)
        unit_input = st.number_input("Enter unit:", min_value=0.0)
        result = calculate_percentage(volume_input, unit_input)

    elif choice == "Unit":
        volume_input = st.number_input("Enter volume:", min_value=0.0)
        percentage_input = st.number_input("Enter percentage:", min_value=0.0)
        result = calculate_unit(percentage_input, volume_input)

    st.write(f"The calculated value is: {result}")

if __name__ == "__main__":
    main()
