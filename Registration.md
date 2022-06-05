from tkinter import *
root =Tk()
root.geometry("500x300")

def getvals():
    print("Accepted")

Label(root, text="Python Registration Form", font="ar 15 bold").grid(row=0, column=3)
name = Label(root, text="Name")
Phone = Label(root, text="Phone")
Gender = Label(root, text="Gender")
Payment = Label(root, text="Payment")
Emergency = Label(root, text="Emergency")

name.grid(row=1, column=2)
Phone.grid(row=2, column=2)
Gender.grid(row=3, column=2)
Payment.grid(row=4, column=2)
Emergency.grid(row=5, column=2)

namevalue= StringVar
Phonevalue= StringVar
Gendervalue= StringVar
Emergencyvalue= StringVar
Paymentvalue= StringVar
checkvalue= IntVar

nameentry = Entry(root, textvariable =namevalue)
Phoneentry = Entry(root, textvariable =Phonevalue)
Genderentry = Entry(root, textvariable =Gendervalue)
Emergencyentry = Entry(root, textvariable =Emergencyvalue)
Paymententry = Entry(root, textvariable =Paymentvalue)

nameentry.grid(row=1, column=3)
Phoneentry.grid(row=2, column=3)
Genderentry.grid(row=3, column=3)
Emergencyentry.grid(row=4, column=3)
Paymententry.grid(row=5, column=3)

checkbtn = Checkbutton(text="remember me?", variable=checkvalue)
checkbtn.grid(row=6, column=3)

Button(text="submit", command=getvals).grid(row=7, column=3)



root.mainloop()