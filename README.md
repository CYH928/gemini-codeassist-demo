# Gemini Code Assist Demo

### Step 1. Install python virtual environment
Ask Gemini: `How to install python venv call ".venv"`
#### Expect Gemini Respond
Linux and MacOS:
```shell
python3 -m venv .venv
source venv/bin/activate
```
Windows:
```shell
python -m venv .venv
venv\Scripts\activate.bat
```
Activated the python virtual environment

---
### Step 2. Explain the code
1. Select **main.py**.
2. In the IDE activity bar, click `Gemini Code Assist Logo`
3. Click **`Explain this`**
#### Expect Gemini Respond
- Dependencies
- Application setup
- Routes
- Application execution
4. In the editor, select the function definition, click the `bulb`, and then click **`Gemini: Explain this`**.

---
### Step 3. Run the app
1. Confirm start the **virtual environment**, Ask Gemini: `How to activate the .venv`
2. Use `@` to add the `main.py` file.
3. Ask Gemini: `@main.py` `How to run the flask app`
#### Expect Gemini Respond
<!-- Linux and MacOS: -->
```shell
python3 main.py
```
<!-- Windows:
```shell
python main.py
``` -->
4. The command returns an error saying there is no module named `flask`.
5. Ask Gemini: 
```
How to slove this problem ?
ModuleNotFoundError: No module named 'flask'
```
6. Ask Gemini: `@requirements.txt` `How do you install Python requirements?`
#### Expect Gemini Respond
```shell
pip install -r requirements.txt
```
7. Run it again `python3 main.py`
8. Test the Roman Numerals web app

---
### Step 4. Add unit tests
1. Open the `calendar.py`
2. Add the `@main.py` and `@calendar.py` files.
3. Select all function codes, click the `bulb`, and then click **`Generate unit tests`**.
4. Create a new file call `test_calendar.py`
5. After, in the Gemini Code Assist click the `Accept changes` or `Insert in current file` button.
6. Run the `test_calendar.py` Python file.

---
### Step 5. Fix the code and make it more readable
1. Open the `calendar.py`
2. Ask Gemini: `@calendar.py` `Make my code more readable and fix any errors`
3. Click the `Toggle view` to view the before and after.
4. Then, click the `Preview in diff mode`, and click `Accept` changes code.

