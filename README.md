
# Practical Git and GitHub Task: Emulating Work at School and Home

### Objective:
Learn how to manage a project locally and with GitHub by simulating working from two different locations: **school** (folder `school`) and **home** (folder `home`). You will practice creating a repository, committing changes, pushing them to GitHub, and then syncing changes between two locations.

---

### Instructions:

#### 1. Set up the **School Environment**:

1. Create a folder named `school` on your local machine.
2. Navigate into the `school` folder in the terminal and initialize a new Git repository:
   ```bash
   git init
   ```
3. Create a `.gitignore` file to ignore unnecessary files:
   - Open `.gitignore` and add:
     ```
     *.log
     node_modules/
     ```
4. Create a new file `index.html` and add basic HTML content.
Use `image.png` as a reference for the structure and design of your HTML file. You'll replicate the layout and styling using HTML and CSS (flexbox).

5. Stage and commit your changes:
   ```bash
   git add .
   git commit -m "Initial commit with basic HTML structure"
   ```

6. Create an **empty repository on GitHub** (without a README or `.gitignore`).

7. Add the GitHub remote repository to your local project:
   ```bash
   git remote add origin <your-repo-URL>
   ```

8. Verify that the remote repository is set correctly:
   ```bash
   git remote -v
   ```

9. Push your local changes to GitHub:
   ```bash
   git push -u origin master
   ```

---

#### 2. Set up the **Home Environment**:

1. On your home machine (or a different folder named `home`), clone the GitHub repository into a new folder:
   ```bash
   git clone <your-repo-URL>
   ```

2. Navigate into the cloned repository (`home` folder):
   ```bash
   cd <repo-folder>
   ```

3. Add a new file `styles.css` to the project and link it to the `index.html` file.

4. Stage and commit your changes:
   ```bash
   git add .
   git commit -m "Added CSS for product card styling"
   ```

5. Push the changes to the GitHub repository:
   ```bash
   git push origin master
   ```

---

#### 3. Returning to the **School Environment**:

1. In the `school` folder, pull the latest changes from the GitHub repository:
   ```bash
   git pull origin master
  ```
2. Check the commit history using `git log` to verify all changes are recorded:
   ```bash
   git log
   ```
3. Continue working on the project. For example, add new content or improve the design in the `index.html` file.

4. Stage and commit the new changes:
   ```bash
   git add .
   git commit -m "Improved product card content"
   ```

5. Push the new changes to GitHub:
   ```bash
   git push origin master
   ```

---

### Git Commands to Use:
- `git init`: Initialize a new Git repository.
- `git add .`: Stage all changes.
- `git status`: Check the status of the repository.
- `git commit -m "message"`: Commit changes with a message.
- `git remote -v`: View the remote repository's details.
- `git remote add origin <URL>`: Add a remote repository.
- `git push origin master`: Push changes to the GitHub repository.
- `git pull origin master`: Pull the latest changes from GitHub.
- `git log`: View commit history.

---

### Final Task:
Ensure that both your **school** and **home** environments are synced with GitHub by committing and pulling changes regularly. Make sure that your page is styled appropriately using **CSS Flexbox** for layout management.
