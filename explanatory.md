# Beginner Explanatory Guide: Exercise 7: Terminal, Testing & Git

> **Task Type**: Service Task  
> **Domain/Focus**: Terminal Navigation, Testing, Git Basics

---

## 1. The Goal (In-Depth Beginner Explanation)

### The Core Problem
In the world of software development, understanding how to navigate the terminal, run tests, and use version control systems like Git is crucial. This exercise addresses the foundational skills necessary for any developer, regardless of the programming language they are using. Currently, many beginners struggle with these essential tools, which can lead to confusion and inefficiency when working on coding projects. Without a solid grasp of terminal commands, developers may find it challenging to manage files, run tests, and collaborate with others effectively.

The importance of this exercise cannot be overstated. Mastering terminal navigation allows developers to interact with their operating system more efficiently, while running tests ensures that the code behaves as expected. Git, on the other hand, is vital for tracking changes, collaborating with others, and maintaining a history of the project. By completing this exercise, you will build a strong foundation that will serve you well throughout your coding journey.

### Jargon Buster (Key Terms Explained)
* **Terminal**: A terminal is a text-based interface that allows users to interact with the operating system by typing commands. For example, using the command `ls` in a terminal will list all files and directories in the current directory. This is much faster than navigating through a graphical user interface (GUI).

* **Testing**: In software development, testing refers to the process of executing code to ensure it behaves as expected. For instance, using a testing framework like `pytest` in Python allows developers to write tests that automatically check if functions return the correct values. If a test fails, it indicates that there is a bug in the code that needs to be fixed.

* **Git**: Git is a version control system that tracks changes in files and allows multiple people to collaborate on a project. For example, when you make changes to a file and use the command `git commit`, Git saves a snapshot of your changes along with a message describing what you did. This helps keep a history of the project and makes it easier to revert to previous versions if needed.

* **Branching**: Branching in Git allows developers to create separate lines of development within a project. For example, if you want to add a new feature without affecting the main codebase, you can create a new branch using `git checkout -b new-feature`. This way, you can work on the feature independently and merge it back into the main branch once it's complete.

### Expected Outcome
After completing this exercise, you should be able to confidently navigate the terminal, run tests for your code, and use Git to manage your projects. 

**Before vs. After**:
- **Before**: You may struggle to find files, run tests, or understand how to track changes in your code.
- **After**: You will be able to navigate directories, execute commands to run tests, and use Git to commit changes, create branches, and collaborate with others effectively.

---

## 2. Related Coding Concepts & Syntax (50% Theory, 50% Practice)

### Concept 1: Terminal Commands
#### 📘 Theoretical Overview (50%)
Terminal commands are the instructions you give to your operating system through a command-line interface. They allow you to perform various tasks such as navigating directories, managing files, and executing programs. Understanding these commands is essential because they provide a powerful way to interact with your computer without relying on a graphical interface. If you do not know how to use terminal commands, you may find it difficult to perform tasks quickly and efficiently.

Key mechanisms include:
- **Navigation**: Commands like `cd` (change directory) allow you to move between folders.
- **File Management**: Commands like `ls` (list) and `rm` (remove) help you view and delete files.
- **Execution**: You can run scripts or programs directly from the terminal, which is often faster than using a GUI.

#### 💻 Syntax & Practical Examples (50%)
* **Language Syntax**:
  ```bash
  # Change to the Product-Track directory
  cd Product-Track
  
  # List all files in the current directory
  ls -la
  ```

* **Real-World Application**:
  ```bash
  # Navigate to Exercise-1 and list files
  cd Product-Track/Week-0/Exercise-1
  ls
  ```

### Concept 2: Git Basics
#### 📘 Theoretical Overview (50%)
Git is a distributed version control system that allows developers to track changes in their codebase. It is essential for collaboration, as it enables multiple developers to work on the same project without overwriting each other's changes. Git keeps a history of all changes, making it easy to revert to previous versions if necessary. Without Git, managing code changes in a team environment would be chaotic and error-prone.

Key mechanisms include:
- **Commits**: Each commit is a snapshot of your project at a specific point in time.
- **Branches**: Branches allow you to work on features or fixes in isolation from the main codebase.
- **Merging**: Once changes are complete, branches can be merged back into the main branch, integrating new features or fixes.

#### 💻 Syntax & Practical Examples (50%)
* **Language Syntax**:
  ```bash
  # Initialize a new Git repository
  git init
  
  # Stage changes for commit
  git add .
  
  # Commit changes with a message
  git commit -m "Initial commit"
  ```

* **Real-World Application**:
  ```bash
  # Create a new branch for a feature
  git checkout -b new-feature
  
  # Make changes, then stage and commit
  git add .
  git commit -m "Add new feature"
  
  # Push changes to the remote repository
  git push origin new-feature
  ```

---

## 3. Step-by-Step Logic & Walkthrough

1. **Step 1: Locate and Analyze the Target File**
   * Open your terminal and navigate to the `s-w00a-exercise-7` folder.
   * Use the command `ls` (or `dir` on Windows) to list the files and locate `INSTRUCTIONS.md` and `README.md`. These files contain essential information about the exercise.

2. **Step 2: Input Verification & Validation**
   * Ensure you have Python installed on your machine. You can check this by typing `python --version` in the terminal.
   * Verify that you are in the correct directory by using the `pwd` command (or `cd` on Windows) to print your current directory.

3. **Step 3: Core Implementation / Modification**
   * Follow the instructions in `INSTRUCTIONS.md` to practice terminal commands. Start with navigating directories using `cd`, listing files with `ls`, and reading file contents with `cat` or `type`.
   * Move on to running tests by navigating to the appropriate exercise folder and executing the test commands provided.

4. **Step 4: Output Verification & Testing**
   * After running the tests, carefully read the output. Look for any failed tests and understand the error messages provided by the testing framework.
   * If any tests fail, revisit the code to identify and fix the issues, then re-run the tests to ensure they pass.

---

## 4. Detailed Walkthrough of Test Cases

### Test Case 1: Standard / Success Case
* **Description**: This test checks if the function correctly calculates the area of a rectangle.
* **Inputs**:
  ```json
  {
    "length": 5,
    "width": 3
  }
  ```
* **Step-by-Step Execution Trace**:
  1. The function `rectangle_area(5, 3)` is called with the inputs.
  2. The function checks if the inputs are valid (non-negative numbers).
  3. The main logic runs: `area = length * width`, which calculates `5 * 3 = 15`.
  4. Returns the final result of `15`.
* **Expected Output**: `15`

### Test Case 2: Edge Case / Validation Fail
* **Description**: This test checks how the function handles invalid input (negative values).
* **Inputs**:
  ```json
  {
    "length": -5,
    "width": 3
  }
  ```
* **Step-by-Step Execution Trace**:
  1. The function `rectangle_area(-5, 3)` is called with the inputs.
  2. The validation block detects that the length is negative.
  3. The execution is halted early, and an error message is returned: "Length must be non-negative."
* **Expected Output**: "Length must be non-negative."

By following this guide, you will gain a solid understanding of terminal navigation, testing, and Git basics, which are essential skills for any aspiring software developer.