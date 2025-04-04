# Module5-Assignment
#Task-1
try:
    with open("sample.txt", "r") as file:
        for line in file:
            print(line.strip())
except FileNotFoundError:
    print("Error: The file 'sample.txt' does not exist")

#Tash-2
with open("Output.txt", "w") as file:
    user_input = input("Enter data to write into the file: ")
    file.write(user_input + "\n")
with open("Output.txt", "a") as file:
    extra_data = input("Enter additional data to append: ")
    file.write(extra_data + "\n")
with open("Output.txt", "r") as file:
    print("\nFinal content of the file: ")
    print(file.read())

