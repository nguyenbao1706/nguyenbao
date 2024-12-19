import tkinter as tk
root = tk.Tk()
root.title(" Bảng")
label = tk.Label(root, text="Thông tin nhân viên", font=("Arial", 20))
label.place(x = 20, y = 20)

check_var1 = tk.IntVar(value=0)
check_var2 = tk.IntVar(value=0)
def check1():
    if check_var1.get() == 1:
        check_var2.set(0)
def check2():
    if check_var2.get() == 1:
        check_var1.set(0)
check1 = tk.Checkbutton(root, text=" Là khách hàng", variable=check_var1, command=check1)
check1.place( x  = 300, y = 30)
check2 = tk.Checkbutton(root, text=" Là nhà cung cấp", variable=check_var2, command=check2)
check2.place( x = 500, y = 30)

root.title(" Bảng")
label =tk.Label(root, text="Mã", font=("Arial", 10))
label.place(x = 25, y = 60)

root.title(" Bảng")
label = tk.Label(root, text="Tên", font=("Arial", 10))
label.place(x = 200, y = 60)

root.title(" Bảng")
label = tk.Label(root, text = "Ngày sinh", font = ("Arial", 10))
label.place(x = 500, y = 60)

root.title(" Bảng")
label = tk.Label(root, text = "Đơn vị", font = ("Arial", 10))
label.place(x = 25, y = 100)

root.title(" Bảng")
label = tk.Label(root, text = "Giới tính", font = ("Arial", 10))
label.place(x = 700, y = 60)

root.title(" Bảng")
label = tk.Label(root, text = "Ngày cấp", font = ("Arial", 10))
label.place(x = 750, y = 100)

root.title(" Bảng")
label = tk.Label(root, text = "Số CMND", font = ("Arial", 10))
label.place(x = 500, y = 100)

root.title(" Bảng")
label = tk.Label(root, text = "Chức danh", font = ("Arial", 10))
label.place(x = 25, y = 140)

root.title(" Bảng")
label = tk.Label(root, text = "Nơi cấp", font = ("Arial", 10))
label.place(x = 500, y = 140)

labels =[ "vb"]
for i, label in enumerate(labels):
    entry = tk.Entry(root, width=17, font=("Arial", 12))
    entry.place(x=25, y=80)

labels =[ "vb"]
for i, label in enumerate(labels):
    entry = tk.Entry(root, width=17, font=("Arial", 12))
    entry.place(x=200, y=80)

labels =[ "vb"]
for i, label in enumerate(labels):
    entry = tk.Entry(root, width=17, font=("Arial", 12))
    entry.place(x=500, y=80)

labels =[ "vb"]
for i, label in enumerate(labels):
    entry = tk.Entry(root, width=37, font=("Arial", 12))
    entry.place(x=25, y=120)

labels =[ "vb"]
for i, label in enumerate(labels):
    entry = tk.Entry(root, width=25, font=("Arial", 12))
    entry.place(x=500, y=120)

labels =[ "vb"]
for i, label in enumerate(labels):
    entry = tk.Entry(root, width=17, font=("Arial", 12))
    entry.place(x=750, y=120)

labels =[ "vb"]
for i, label in enumerate(labels):
    entry = tk.Entry(root, width=37, font=("Arial", 12))
    entry.place(x=25, y=160)

labels =[ "vb"]
for i, label in enumerate(labels):
    entry = tk.Entry(root, width=45, font=("Arial", 12))
    entry.place(x=500, y=160)


def on_select():
    if var.get() == 1:
        print("Đã chọn")
    else:
        print("Chưa chọn")
root.title("Ô Tròn Tích")
var = tk.IntVar()
radiobutton = tk.Radiobutton(root, text="Nam", variable=var, value=1, command=on_select, indicatoron=True)
radiobutton.place(x = 700 , y = 80)
radiobutton2 = tk.Radiobutton(root, text="Nữ", variable=var, value=0, command=on_select, indicatoron=True)
radiobutton2.place(x = 760 , y = 80)

root.mainloop()
