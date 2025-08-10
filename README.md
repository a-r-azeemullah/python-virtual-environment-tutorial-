🐍 Creating a Python Virtual Environment (Without Disturbing Others)

When working on Python projects, it's best to use a virtual environment so your dependencies are isolated and don't interfere with other projects.

------------------------------------------------------------
📌 Steps to Create and Use a Virtual Environment
------------------------------------------------------------

1️⃣ Navigate to Your Project Folder:
    cd path/to/your/project

2️⃣ Create the Virtual Environment:
    python3 -m venv venv

3️⃣ Activate the Virtual Environment:
    source venv/bin/activate

💡 Once activated, you’ll see (venv) appear at the start of your terminal prompt.

4️⃣ Deactivate the Virtual Environment:
    deactivate


------------------------------------------------------------
📦 Managing Dependencies with requirements.txt
------------------------------------------------------------

📥 Save all installed libraries into a requirements.txt file:
    pip freeze > requirements.txt

📤 Recreate the same environment elsewhere:
    pip install -r requirements.txt


------------------------------------------------------------
🚫 Ignoring the venv Folder in GitHub
------------------------------------------------------------

You should NOT upload the venv folder to GitHub.  
Instead, use a .gitignore file.

Create .gitignore:
    touch .gitignore

Add the following inside .gitignore:
    venv/

✅ This keeps your repository clean and avoids uploading unnecessary files.


------------------------------------------------------------
🚀 Pushing Your Project to GitHub
------------------------------------------------------------

    git init
    git add .
    git commit -m "Initial commit with example script"
    git branch -M main
    git remote add origin https://github.com/<your-username>/<repo-name>.git
    git push -u origin main


------------------------------------------------------------
📊 Flow Diagram (Mermaid format for README.md)
------------------------------------------------------------

    ```mermaid
    graph TD;
        A[Start Project] --> B[Create Virtual Environment];
        B --> C[Activate Environment];
        C --> D[Install Packages];
        D --> E[Export requirements.txt];
        E --> F[Add venv to .gitignore];
        F --> G[Push to GitHub];
        G --> H[Done ✅];
    ```

------------------------------------------------------------

💡 Pro Tip: Keep your requirements.txt updated so others can easily replicate your setup.
