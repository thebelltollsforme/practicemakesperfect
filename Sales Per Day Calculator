#This program requests salesperson names, length of sales period, and quantity of sales, then outputs the information of name, sales, and average sales in the console and also into a document.  Checks to make sure that invalid information isn't placed.


f = open("statsdoc.txt","w")
database = {}
name = "empty"
verficationtoggle = "empty"
namelist = []
print(name)
while name.lower() != "q" and name.lower() != "quit":
    name = input("Enter salesperson name.  When done, type Quit or Q: ")
    if name.lower() == "q" or name.lower() == "quit":
        break
    print ("is {0} the name?".format(name))
    verificationtoggle = input("Y or N: ")
    if verificationtoggle.lower() == "y" or verificationtoggle.lower() == "yes":
        namelist.append(name)
    else:
        print("Please re-enter name")

tpinput = input("Please enter the sales period, in days: ")
while tpinput.isdigit() == False:
    tpinput = input("That is not an applicable number.  Please re-enter the number of days: ")


for i in namelist:
    print(i)
    placeholder = input("Enter sales dollars for salesperson: ")
    while placeholder.isdigit() == False:
        placeholder = input("Please re-enter, invalid number: ")
    database[i] = placeholder
print("Name", end ="    ")
print("Sales", end ="    ")
print("Average Sales Per Day")
f.write("Name")
f.write("    ")
f.write("Sales")
f.write("    ")
f.write("Average Sales Per Day")
f.write(" \n")

for b in database:
    print(b, end="   ")
    print(database[b], end ="   ")
    divisionres = int(database[b])/int(tpinput)
    print(divisionres)
    f.write(str(b))
    f.write("    ")
    f.write(str(database[b]))
    f.write("    ")
    f.write(str(divisionres))
    f.write(" \n")

#print(tpinput)
#print(namelist)
print(database)
