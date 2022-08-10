print(" ")

print("----------------------------------------------------")
print("******* WELCOME TO STUDENT MANAGEMENT SYSTEM *******")

sms=["kamlesh", "amit","dinesh"]

def viewname():
    for i in range(len(sms)):
                   print(sms[i])

def addname():
    a=input("Enter the New Student name : ")
    sms.append(a)
    print("Student name added")

def removename():
    a=input("Search Student name : ")
    if a in sms:
        sms.remove(a)
        print("Removed Student name")
    else:
        print("Student not found")

def searchname():
    a=input("Search Student name : ")
    if a in sms:
        print("Student found")
    else:
        print("Student not found")

while(True):
    print("----------------------------------------------------")
    print("Please choose any one options:")
    print("1. To view student list")
    print("2. To add new list")
    print("3. To remove the data")
    print("4. To serach data")
    print("5. Exit")

    ch=int(input("Enter your Chooes : "))

    if ch==1:
        viewname()
    elif ch==2:
        addname()
    elif ch==3:
        removename()
    elif ch==4:
        searchname()
    elif ch==5:
        exit()
    else:
        print("Wrong Entry")

    c=input("Do you want to continue y/n :")

    if(c=="y"):
        continue
    elif(c=="n"):
        break
