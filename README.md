**NutriFit - An Algorithmic Health & Nutrition Analytics Engine**

Hii everyone, this is my mini project for calculating health stuffs like BMI, BMR, TDEE and Bodyfat percentage. I made this in python becuase it was easy to make calculator type programs with functions and if-else. Below i have given all the steps how to run this project even if you dont know anything about it.

**What this project does**

This is a simple menu-driven program (means it keeps asking you what you wanna do untill you exit). It have 4 main features:

1. **BMI Calculator** - tells you your Body Mass Index and wheter your underweight, healthy, overweight or obese.
2. **BMR Calculator** - calculates your Basal Metabolic Rate (the calories your body burn while doing nothing, like resting)
3. **TDEE Calculator** - Total Daily Energy Expenditure, basically BMR multiplied by your activity level
4. **Bodyfat Calculator** - estimates your body fat percentage acording to your age and gender category

**Requirements (Enviroment Setup)**

Before running this project make sure you have the folowing:

- Python 3 installed in your system (any version above 3.6 should work fine, i used 3.11 while makeing this)
- A terminal / command prompt (cmd, powershell, or bash - anything works)
- No internet connection needed, its fully offline
- No extra libraries required!! This project only uses built in python stuff, so no need to pip install anything extra. (i know thats rare lol)

**How to check if python is installed**

Open your terminal and type this - python --version

or if that dont work try - python3 --version

If you see something like Python 3.11.4 that means your good to go. If it says command not found, you need to download python first from the offical website: https://www.python.org/downloads/ and install it (make sure to tick the "Add python to PATH" checkbox during install, i forgot that once and it took me 1 hour to fix lol).

**Installation / Setup Steps**

1. Download or clone this repository/project folder to your computer.
2. Make sure the main python file (lets say its named nutrifit.py or whatever you saved it as) is in a folder you can easily navigate to.
3. Open your terminal/cmd.
4. Navigate to the folder where the file is kept using cd command. Example - cd Desktop/NutriFit
   (change the path acording to were you actully saved the file, this is just an example i used my own folder name)
5. Thats basically it for setup, no dependencies to install seperatly since we only used standard python libraries.

**How to Run the Project**

Once your in the correct folder, just type this command and hit enter - python nutrifit.py

or incase that dosent work, try - python3 nutrifit.py

(the file name might be different for you depending what you saved it as, just replace nutrifit.py with your actual filename)

After runing this, a menu will pop up in your terminal, it will show the project title on top and then 5 options below it - BMI, BMR, TDEE, Bodyfat and Exit, each having a number infront of it (1,2,3,4 and 0). Below that it will ask "Enter a choice:" and thats were you type your number.

Now you just enter the number acording to what you wanna calculate and press enter.

**How to use each option (Configuration/Inputs needed)**

**Option 1 - BMI**
- It will ask for height (in metres, not cm! like 1.75 not 175)
- Then ask for weight (in kg)
- It gives your BMI value and tells you the category (underweight/healthy/overweight/obese)

**Option 2 - BMR**
- First it asks gender, type exactly male or female, all small letters (other spellings wont work as this is case sensitive)
- Then height (this one needs to be in cm, confusing i know but thats how the formula works mathematically)
- Then weight in kg
- Then your age
- It gives you the BMR in kilocalories per day

**Option 3 - TDEE**
- Same as BMR inputs (gender, height in cm, weight, age)
- After that it asks for your activity level, you have to type it exactly as shown below otherwise it will say invalid input:
  - Sedentary
  - Lightly Active
  - Moderately Active
  - Very Active
  - Extra Active
  (spelling and capital letters matter here, so type carefully)
- It then gives your TDEE which is basically how many calories you burn in a day including activity

**Option 4 - Bodyfat**
- Ask for gender catagory, type exactly one of these (again capital letters matter):
  - Adult male
  - Adult female
  - Boy
  - Girl
- Then height (in meters, since it uses BMI formula internaly) and weight in kg
- Then age
- Gives your estimated bodyfat percentage

**Option 0 - Exit**
- Just closes the program, prints "Thank you" and stops runing.

**Common Mistakes / Troubleshoot**

- If you enter a letter/text where a number was expected (like typing "twenty" instead of "20") the program will crash, so always enter proper numbers only.
- Remember gender inputs are case-sensitive, Male or MALE wont work, has to be male (all small letters).
- If choice number is invalid it just prints "Enter a valid choice" and loops back to menu again, no crash there atleast.
- Height units differ between options (metres for BMI/Bodyfat, cm for BMR/TDEE) so dont get confused, this tripped me up during testing too.

**Notes**

This project was made for learning purpose only, the bodyfat and BMR formulas used are standard ones found online (Mifflin-St Jeor equation for BMR, and standard BMI based estimation for bodyfat), so results are just a estimate and not a substitute for actual medical/proffesional advice.

Thats it! Thanks for checking out my project, hope the instructions were clear enough 😅
