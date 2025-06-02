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

---
### Step 6. Enhance code readability for non-native English users
1. Open the `main.py`
2. Ask Gemini: `@main.py` `Add comments to main.py`
But what if English is not your first language?
3. Ask Gemini: `Add Spanish comments to main.py`
4. Click the `Preview in diff mode`, and click `Decline` changes code.

---
### Step 7. Improve how the app looks
1. Run `python3 main.py` in the terminal, click **Open Preview**.
2. Open the `templates/index.html`
3. Ask Gemini: `@index.html` `Make the CSS style for this HTML template look more better`
4. Then, click `Accept changes` button.
5. Refresh and back to the **Preview** web page
6. After, ask the Gemini `@convert.html` `Make it template look similar to the` `@index.html`
4. Click the `Preview in diff mode`, and click `Accept` changes code.
4. Finally, click `Accept` button to save the chaged code.

---
### Step 8. Enable the Tools
1. Ask Gemini `@GoogleDocs` `List my docs`
2. First time to use, will need the enable the **Tools**, Click the `Click here to enable GoogleDocs`
3. The GoogleDocs part click the `Enable`, select the region `asia-east1 (Taiwan)`, and then click `Enable`
4. Click `Connect`
Successfully connected to the Tools.

---
### Step 9. Use the Google Docs Tool
1. Ask Gemini `@GoogleDocs` `List my docs`
2. Ask Gemini `@GoogleDocs` `Find docs titled` `<keyword>`(todo)
3. Ask Gemini `@GoogleDocs` `Find docs containing` `<keyword>` (api)
4. Ask Gemini `@GoogleDocs` `Summarize doc` `<docs_name>` (Todo Apps)
5. Ask Gemini `@GoogleDocs` `Get doc` `<docs_name>` (Todo Apps)
6. Click open the `main.py` and select `Current file` or use `@` to add the files / folders
7. Ask Gemini `Generate the flask app with API`
8. Run `python3 main.py` in terminal, and open Preview Page.
9. Press **Ctrl+i**, and input /generate `Create some data`, and click `Accpet` button.

---
Step 8. Use the GitHub Tool
1. Ask Gemini `@GitHub` `List my issues`
2. Ask Gemini `@GitHub` `List top issues for project` `<project_name>` (ITP4115 EA)
1. Ask Gemini `@GitHub` `List my open pull requests`
1. Ask Gemini `@GitHub` `List my pull requests`