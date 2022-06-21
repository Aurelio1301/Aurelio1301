- 👋 Hi, I’m @Aurelio1301
- 👀 I’m interested in programming
- 🌱 I’m currently learning Clean Code
- 💞️ I’m looking to collaborate on laptop
- 📫 How to reach me Call me on whatsapp (+6281393007972)

<!---
Aurelio1301/Aurelio1301 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

Calculator

def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y
    
def divide(x, y):
    return x / y


print("Select operation.")
print("1. +")
print("2. -")
print("3. *")
print("4. /")

while True:
    choice = input("Enter choice(1/2/3/4): ")

    if choice in ('1', '2', '3', '4'):
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))

        if choice == '1':
            print(num1, "+", num2, "=", add(num1, num2))

        elif choice == '2':
            print(num1, "-", num2, "=", subtract(num1, num2))

        elif choice == '3':
            print(num1, "*", num2, "=", multiply(num1, num2))

        elif choice == '4':
            print(num1, "/", num2, "=", divide(num1, num2))
        
        next_calculation = input("Let's do next calculation? (yes/no): ")
        if next_calculation == "no":
          break
    
    else:
        print("Invalid")
