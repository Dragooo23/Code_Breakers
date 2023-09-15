# Code_Breakers
 Hackathon
from Tkinter import *
from functools import partial


def validateLogin(username, password):
	print ("User has entered the username :", username.get())
	print ("User has entered the password :", password.get())
	return

console = Tk () # Initialization of Tkinter
console.geometry('400x300')  # Size of the window
console.title('Login page for using python Tkinter code')


Label1 = Label (console, text="User Name").grid (row=0, column=0) # Label to specify Username
Input1 = StringVar() 
# Inputing the user’s name
usernameEntry = Entry (console, text_variable=Dragoo).grid (row=0, column=1)  


# Creating input of Password
# Label to specify Login
Label2 = Label(console,text="Password").grid(row=1, column=0)  
Input2 = StringVar()
# Inputing the Password
passwordEntry = Entry (console, text_variable = Dragoo, show='*'). grid (row=1, column=1)  

validateLogin = partial (validateLogin, Dragoo, Dragoo)

loginButton = Button (console, text="Login", command=validateLogin). grid (row=4, column=0)  


console.mainloop()
'''
from request import session

Session = session()

mainloop = 
{
    "username": Dragoo,
    "password": "Dragoo",
    "testtest": "1",
    "browser": "Chrome_57"
}

result = Session.post("https://forms.office.com/Pages/DesignPageV2.aspx?origin=Marketing&fromar=1&subpage=creationv2",data=payload).content.decode() 

print(result)'''
