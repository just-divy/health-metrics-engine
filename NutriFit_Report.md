**Project Report - NutriFit (Health & Nutrition Calculator)**

**Name of Project:** NutriFit - An Algorithmic Health & Nutrition Analytics Engine

**Made By:** Divya Raj SIngh

**Language Used:** Python

---

**1. Introduction**

For my project i decided to make a health calculator becuase health and fitness is something everyone is intrested in nowdays, and also i wanted to practice python functions and if-else statements properly. So i made a small program called NutriFit which can calculate 4 diffrent health related things - BMI, BMR, TDEE and Bodyfat percentage. Its a simple terminal based program, meaning it dont have any fancy graphics or buttons, you just run it in cmd/terminal and it ask you questions and gives you answers based on wat you type.

**2. Objective**

The main objective of this project was to:
- Learn how to use functions properly in python (i made seperate functions for each calculation like bmi(), bmr_for_male(), bmr_for_female())
- Practice using if-elif-else statements for decison making
- Make a program that is actully useful in real life, not just a random example
- Understand how loops work by using a while loop to keep the menu running untill user exits

**3. Tools and Technology Used**

- Python 3 (thats the only language used)
- No external libraries needed, only the built in stuff that comes with python
- Any normal text editor or IDE to write the code (i used a simple code editor)
- Terminal/Command prompt to run and test the program

**4. Features of the Project**

The program have a menu with 5 options:

1. **BMI Calculator** - takes height (in meters) and weight (in kg) and tells you your Body Mass Index, also tells if your underweight, healthy, overweight or obese depending on the value.
2. **BMR Calculator** - takes gender, height, weight and age, then calculates Basal Metabolic Rate which is basically how many calories your body burns just by resting (not doing any activity).
3. **TDEE Calculator** - this one first calculates BMR same as above, then multiplies it with a activity factor depending on how active the person is (like sedentary, lightly active, etc) to get Total Daily Energy Expenditure.
4. **Bodyfat Calculator** - estimates body fat percentage using a formula that need BMI and age, and it changes slightly depending on if the person is Adult male, Adult female, Boy or Girl.
5. **Exit option** - just closes the program when your done.

**5. How the Program Works (Methodology)**

The program runs inside a while True loop so that the menu keeps showing again and again untill the user choose to exit. Based on wat number the user enters (1,2,3,4 or 0) the program goes into a diffrent if-elif block and ask for the relevent inputs.

For calculations i made seperate functions:
- bmi(a,b) - calculates bmi using the formula weight divided by height squared
- bmr_for_male(w,h,a) - calculates bmr for males using the Mifflin-St Jeor formula
- bmr_for_female(w,h,a) - same formula but diffrent constant since the formula is slightly diffrent for females

For TDEE i just took the BMR value and multiplied it by a number depending on activity level (like 1.2 for sedentary, 1.375 for lightly active and so on, these numbers are standard values used in real fitness calculators too, i found them online).

For bodyfat i used a diffrent formula that uses BMI value and age, and the constant numbers change a bit for male/female/boy/girl catagories.

**6. Sample Working**

When you run the program it shows a menu like this:

NutriFit Analytics Engine Main Menu with options 1 to 4 and 0 to exit. User types a number, program asks the required inputs one by one like height, weight, age, gender etc, and then it shows the calculated result with a proper message.

**7. Challenges Faced**

- Understanding the diffrent formulas for BMR and Bodyfat took some time since they use diffrent constants for male/female.
- Making sure the user enters things in the exact spelling/case (like typing "male" in small letters only) was a bit tricky to explain to the user, i had to be careful about that in my instructions.
- Also had to remember which option needs height in meters and which one needs it in centimeters, that confused me a little while testing.

**8. Limitations**

- The program dont check if the input is valid before using it, so if user enters wrong type of data (like text instead of number) it will crash.
- The formulas used are just estimates, they are not 100% accurate for every body type and shouldnt be used as actual medical advice.
- There is no way to save your past results, every time you run it it starts fresh.

**9. Conclusion**

Overall this project helped me understand functions, loops and conditonal statements better in python. It also gave me a chance to work on something practical thats actully useful and not just a boring example program. In future i want to improve it by adding input validation and maybe saving user history to a file so people can track there progress over time.

**10. How to Run**

The full instructions for running this project is given in the README file, but in short you just need python installed and then run the program using python nutrifit.py from your terminal, no extra installation needed since it dont use any external libraries.

---

Thats my report, thanks for reading!
