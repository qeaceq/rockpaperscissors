# rockpaperscissors
# There are 6 options for this game but ı wonder how can ı write if there are many. Arguments are in Turkish btw.
import random
import tkinter
from tkinter import simpledialog

ROOT = tkinter.Tk()
ROOT.withdraw()
C = simpledialog.askstring(title="Taş Kağıt Makas",
                                  prompt="Seçiminiz:")
A = ["Taş","Kağıt","Makas"]
B = random.choice(A)
if C == B:
    tkinter.messagebox.showwarning(title="Sonuç", message=f"Berabere, Bilgisayarın Seçimi:{B}")
if C == "Taş" and B == "Kağıt":
    tkinter.messagebox.showwarning(title="Sonuç", message=f"Bilgisayar Kazandı, Bilgisayarın Seçimi:{B}")
if C == "Taş" and B == "Makas":
    tkinter.messagebox.showwarning(title="Sonuç", message=f"Kazandınız!, Bilgisayarın Seçimi:{B}")
if C == "Kağıt" and B == "Makas":
    tkinter.messagebox.showwarning(title="Sonuç", message=f"Bilgisayar Kazandı, Bilgisayarın Seçimi:{B}")
if C == "Kağıt" and B == "Taş":
    tkinter.messagebox.showwarning(title="Sonuç", message=f"Kazandınız!, Bilgisayarın Seçimi:{B}")
if C == "Makas" and B == "Taş":
    tkinter.messagebox.showwarning(title="Sonuç", message=f"Bilgisayar Kazandı, Bilgisayarın Seçimi:{B}")
if C == "Makas" and B == "Kağıt":
    tkinter.messagebox.showwarning(title="Sonuç", message=f"Kazandınız!,Bilgisayarın Seçimi:{B}")
