# Hackathon-143
import tkinter as tk
from tkinter import messagebox

# --- Functions ---
def open_account():
    messagebox.showinfo("Open Account", "Opening a new account...")

def deposit_money():
    messagebox.showinfo("Deposit", "Deposit money into account...")

def withdraw_money():
    messagebox.showinfo("Withdraw", "Withdraw money from account...")

def check_balance():
    messagebox.showinfo("Balance", "Checking account balance...")

# --- Main Window ---
root = tk.Tk()
root.title("Bank Management System")
root.geometry("400x300")

# Heading
title_label = tk.Label(root, text="Bank Management System", font=("Arial", 16, "bold"))
title_label.pack(pady=10)

# Buttons
btn_open = tk.Button(root, text="Open New Account", width=20, command=open_account)
btn_open.pack(pady=5)

btn_deposit = tk.Button(root, text="Deposit Money", width=20, command=deposit_money)
btn_deposit.pack(pady=5)

btn_withdraw = tk.Button(root, text="Withdraw Money", width=20, command=withdraw_money)
btn_withdraw.pack(pady=5)

btn_balance = tk.Button(root, text="Check Balance", width=20, command=check_balance)
btn_balance.pack(pady=5)

btn_exit = tk.Button(root, text="Exit", width=20, command=root.quit)
btn_exit.pack(pady=20)

root.mainloop()
