Project 1: Simple Calculator

def add(a, b): return a + b

def subtract(a, b): return a - b

def multiply(a, b): return a * b

def divide(a, b): if b == 0: return "Error: Division by zero" return a / b

Project 2: Basic To-Do List

todo_list = []

def add_task(task): todo_list.append(task) return f'Task "{task}" added.'

def remove_task(task): if task in todo_list: todo_list.remove(task) return f'Task "{task}" removed.' return "Task not found."

def view_tasks(): return "\n".join(todo_list) if todo_list else "No tasks available."

Project 3: Number Guessing Game

import random

def guessing_game(): number_to_guess = random.randint(1, 100) attempts = 0 while True: try: guess = int(input("Guess a number between 1 and 100: ")) attempts += 1 if guess < number_to_guess: print("Too low!") elif guess > number_to_guess: print("Too high!") else: print(f"Congratulations! You guessed it in {attempts} attempts.") break except ValueError: print("Please enter a valid number.")

Project 4: Simple Contact Book

contacts = {}

def add_contact(name, phone): contacts[name] = phone return f"Contact {name} added."

def remove_contact(name): if name in contacts: del contacts[name] return f"Contact {name} removed." return "Contact not found."

def view_contacts(): return "\n".join([f"{name}: {phone}" for name, phone in contacts.items()]) if contacts else "No contacts available."# 222