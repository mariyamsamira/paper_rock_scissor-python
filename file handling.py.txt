import os
print("#######################################")
print("#         FILE HANDELING              #")
print("#######################################")
def ins():
    print("1. create new file")
    print("2.write text in file")
    print("3.list the file")
    print("4.delet the file")
    print("5. rename the file")

c=int(input("enter ur choice"))
ins()

def create_file():
    name=input("enter the file name:")
    with open(name+".txt","w")as file:
        file.write("welcome")
print("name","created sucessfully...")

def write_file():
    name=input("enter the file name to write:")
    text=input("type the content:")
    with open(name+".txt","a")as file:
        file.write("text")
print("name","writed sucessfully...")



while('True'):
 ins()
 match c:
    case 1:
        print("create new file")
        "craete_file()"
    case 2:
         print("edit")
         'write_file()'
    case 3:
         print("list file")
         direc="."
         file_list=os.listdir(direc)
         print(file_list)
    case 4:
         print("delet file")
         n=("type the file name to delect:")
         os.remove(n)
         print("deleted sucessfully")
    case 5:
         print("rename")
    case 6:
         print("stop the program")