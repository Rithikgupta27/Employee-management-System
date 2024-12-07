max = 20

# Structure of Employee
class employee:
	def __init__(self):
		self.name = ''
		self.code = 0
		self.designation = ''
		self.exp = 0
		self.age = 0

num = 0
emp = [employee() for i in range(max)]
tempemp = [employee() for i in range(max)]
sortemp = [employee() for i in range(max)]
sortemp1 = [employee() for i in range(max)]

# Function to build the given datatype
def build():
	global num, emp

	print("Build The Table")
	print("Maximum Entries can be", max)

	num = int(input("Enter the number of Entries required: "))

	if num > max:
		print("Maximum number of Entries are 20")
		num = 20

	print("Enter the following data:")
	for i in range(num):
		emp[i].name = input("Name: ")
		emp[i].code = int(input("Employee ID: "))
		emp[i].designation = input("Designation: ")
		emp[i].exp = int(input("Experience: "))
		emp[i].age = int(input("Age: "))

	showMenu()

# Function to insert the data into
# given data type
def insert():
	global num, emp

	if num < max:
		i = num
		num += 1

		print("Enter the information of the Employee:")
		emp[i].name = input("Name: ")
		emp[i].code = int(input("Employee ID: "))
		emp[i].designation = input("Designation: ")
		emp[i].exp = int(input("Experience: "))
		emp[i].age = int(input("Age: "))
	else:
		print("Employee Table Full")

	showMenu()

# Function to delete record at index i
def deleteIndex(i):
	global num, emp

	for j in range(i, num - 1):
		emp[j].name = emp[j + 1].name
		emp[j].code = emp[j + 1].code
		emp[j].designation = emp[j + 1].designation
		emp[j].exp = emp[j + 1].exp
		emp[j].age = emp[j + 1].age

# Function to delete record
def deleteRecord():
	global num, emp

	code = int(input("Enter the Employee ID to Delete Record: "))

	for i in range(num):
		if emp[i].code == code:
			deleteIndex(i)
			num -= 1
			break

	showMenu()

def searchRecord():
	global num, emp

	code = int(input("Enter the Employee ID to Search Record: "))

	for i in range(num):
		# If the data is found
		if emp[i].code == code:
			print("Name:", emp[i].name)
			print("Employee ID:", emp[i].code)
			print("Designation:", emp[i].designation)
			print("Experience:", emp[i].exp)
			print("Age:", emp[i].age)
			break

	showMenu()

# Function to show menu
def showMenu():
	print("-------------------------GeeksforGeeks Employee Management System-------------------------\n")
	print("Available Options:\n")
	print("Build Table		 (1)")
	print("Insert New Entry (2)")
	print("Delete Entry	 (3)")
	print("Search a Record	 (4)")
	print("Exit			 (5)")

	# Input Options
	option = int(input())

	# Call
	if option == 1:
		build()
	elif option == 2 :
		insert()
	elif option == 3 :
		deleteRecord()
	elif option == 4 :
		searchRecord()
	elif option == 5 :
		return
	else:
		print("Expected Options")
		print("are 1/2/3/4/5")
		showMenu()
# Driver code
showMenu()
	
