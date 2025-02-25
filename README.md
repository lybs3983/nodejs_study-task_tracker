# nodejs_study-task_tracker
Solve [https://roadmap.sh/projects/task-tracker](https://roadmap.sh/projects/task-tracker) with Node.js + Yarn + TypeScript + VS Code.

## PreRequirements
1. **Install Node.js:**
   - You can download and install the appropriate version from the [Node.js official website](https://nodejs.org/).
   - After installation, you can check the Node.js version with the following command:
     ```bash
     node -v
     ```

2. **Install Yarn:**
   - If you haven't installed Yarn yet, you can install it via npm (the package manager that comes with Node.js):
     ```bash
     npm install -g yarn
     ```
   - Check the Yarn version to confirm successful installation:
     ```bash
     yarn -v
     ```

3. **Add yarn global installation path to environment variables:**
   - Check the yarn global installation path:
     ```bash
     yarn global bin
     ```
   - Add the path to the environment variables: Path or PATH

## How to run
1. **Clone the Repository:**
   ```bash 
   git clone https://github.com/lybs3983/nodejs_study-task_tracker.git
   ```

2. **Navigate to the Project Directory:**
   ```bash
   cd nodejs_study-task_tracker
   ```

3. **Use the following commands to build and link:**
    ```bash
    yarn install  # Install dependencies
    yarn build    # Compile TypeScript code
    yarn link     # Link the CLI tool to the global environment
    ```

4. **Run the CLI commands below or other related commands:**
    ```bash
    # Adding a new task
    task-cli add "Buy groceries"
    # Output: Task added successfully (ID: 1)

    # Updating and deleting tasks
    task-cli update 1 "Buy groceries and cook dinner"
    task-cli delete 1

    # Marking a task as in progress or done
    task-cli mark-in-progress 1
    task-cli mark-done 1

    # Listing all tasks
    task-cli list

    # Listing tasks by status
    task-cli list done
    task-cli list todo
    task-cli list in-progress
    ```