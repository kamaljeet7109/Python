# Python
Programming in Python
Write python program to print first letter of your name 
a) Example: Peter
               *      *
               *             *
               *              *
               *      *
               *
               *
               *
b) Print your name by using for loop

c) check the user name is palindrome or not
ans
def print_initial(name):
    # Print first letter of the name in a stylized format
    initial = name[0].upper()
    print(" " * 5 + "*")
    print(" " * 5 + "*")
    print(" " * 5 + "*")
    print(" " * 5 + "*")
    print("*" * 5)
    print("*" * 5)
    print("*" * 5)
    print(" " * 5 + "*")
    print(" " * 5 + "*")
    print(" " * 5 + "*")
    print(" " * 5 + "*")
    print(" " * 5 + initial)
    print()

def print_name(name):
    # Print name using a for loop
    for letter in name:
        print("*" * 5)
        print("*" + " " * 3 + "*")
        print("*" + letter.upper() + " " * 2 + "*")
        print("*" + " " * 3 + "*")
    print("*" * 5)
    print()

def is_palindrome(name):
    # Check if the user name is palindrome or not
    return name.lower() == name[::-1].lower()

# Example usage
user_name = input("Enter your name: ")
print_initial(user_name)
print_name(user_name)
if is_palindrome(user_name):
    print(f"{user_name} is a palindrome!")
else:
    print(f"{user_name} is not a palindrome.")
