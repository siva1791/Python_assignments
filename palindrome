def is_palindrome(input_string):
    reverse_string = ""
    lis_string = input_string.split(" ")

    for i in lis_string[len(lis_string)-1::-1]:
        reverse_string += i + " "

    if reverse_string[0:len(reverse_string)-1].lower() == input_string.lower():
        return "The given string is palindrome"
    else:
        return "The string is not palindrome"

n = input("Enter the String: ")
print(is_palindrome(n))
