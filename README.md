Step 1: Go to GitHub

Open https://github.com

Log in to your account.

Step 2: Create a New Repository

Click the + icon (top-right) → New repository

Fill in:

Repository name (e.g., my-js-project)

Description (optional)

Public / Private (choose based on your need)

Tick Add a README file (recommended)

(Optional) Add:

.gitignore → choose language (e.g., Python, Node, Java)

License → MIT for open source

Click Create repository

✔ Your repo is ready.

Now you can push code OR open it in Codespaces.

💻 2. Setting Up a GitHub Codespace
6

A Codespace is a full VS Code environment running in the cloud.
No installations → Node, Python, Java, Docker you can run everything.

Step 1: Open Codespace from the Repository

Inside your repo:

Click Code (green button)

Choose Codespaces

Click Create codespace on main

GitHub will start a cloud environment with:

VS Code editor

Integrated terminal

Git support

Extensions (you can install like normal VS Code)

🔧 3. Using the Terminal Inside Codespace
Check if languages are installed:
node -v
python3 --version
gcc --version

Install project dependencies:

Example (Node.js):

npm install
npm start

🌱 4. Basic Git Commands Inside Codespace

Codespaces automatically clones your repo, so you can directly commit & push.

Add changes
git add .

Commit
git commit -m "Initial commit"

Push
git push


You will instantly see the updates in your GitHub repo.

⚙️ 5. Optional: Add a Dev Container (for custom environment)

If you need:

Python + Node

custom tools

specific versions

create a folder:

.devcontainer/devcontainer.json


Example minimal file:

{
  "name": "My Codespace",
  "image": "mcr.microsoft.com/devcontainers/javascript-node:1-18"
}


Codespaces auto-detects this and sets up your environment accordingly.