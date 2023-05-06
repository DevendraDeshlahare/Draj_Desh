# Draj_Desh
# It is just DIGITAL CLOCK small project in python.
from tkinter import Label, Tk 
import time
app_window = Tk() 
app_window.title("Draj Desh") 
app_window.geometry("580x150") 
app_window.resizable(1,1)

text_font= ("Boulder", 68, 'bold')
background = "#f2e750"
foreground= "#363529"
border_width = 25

label = Label(app_window, font=text_font, bg=background, fg=foreground, bd=border_width) 
label.grid(row=0, column=1)

def Draj_Desh(): 
   time_live = time.strftime("%I:%M:%S %p")
   label.config(text=time_live) 
   label.after(200, digital_clock)

Draj_Desh()
app_window.mainloop()
