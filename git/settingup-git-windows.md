# Git Installation and Configuration on Windows

<a name="readme-top"/>

<br/>

<br />
<div align="center">
  <h3 align="center">Git Installation and Configuration on Windows</h3>
</div>
<div align="center">
  A comprehensive guide to installing Git on Windows, configuring it, and integrating with VS Code.
</div>

<br />

---

<br />
<br />

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#installation">Installation</a>
    </li>
    <li>
      <a href="#configuration">Configuration</a>
      <ol>
        <li>
          <a href="#basic-configuration">Basic Configuration</a>
        </li>
        <li>
          <a href="#vs-code-integration">VS Code Integration</a>
        </li>
        <li>
          <a href="#github-repositories">GitHub Repositories</a>
          <ol>
            <li>
              <a href="#clone-a-repository-in-vs-code">Clone a Repository in VS Code</a>
            </li>
            <li>
              <a href="#create-a-new-repository">Create a New Repository</a>
            </li>
          </ol>
        </li>
        <li>
          <a href="#github-issues">GitHub Issues</a>
        </li>
        <li>
          <a href="#github-pull-requests">GitHub Pull Requests</a>
        </li>
      </ol>
    </li>
  </ol>
</details>

---

## Installation

1. **Download Git:**
   - Go to the [Git official website](https://git-scm.com/download/win) and download the latest version for Windows.

2. **Run the Installer:**
   - Locate the downloaded `.exe` file and run it.

3. **Setup Wizard:**
   - Follow the steps in the setup wizard. The default options are usually fine for most users. Pay attention to the following steps:
     - **Select Components:** Ensure "Git Bash Here" and "Git GUI Here" are selected.
     - **Choosing the Default Editor Used by Git:** Select your preferred text editor. If you use VS Code, choose it here.
     - **Adjusting Your PATH Environment:** Select "Git from the command line and also from 3rd-party software".

4. **Finish Installation:**
   - Complete the installation process and verify it by opening a command prompt and typing `git --version`. You should see the installed Git version.

## Configuration

### Basic Configuration

1. **Set Your Username and Email:**
   - Open Git Bash and set your global username and email. These details will be associated with your commits.
     ```sh
     git config --global user.name "Your Name"
     git config --global user.email "youremail@example.com"
     ```

2. **Check Configuration:**
   - Verify your settings with:
     ```sh
     git config --list
     ```

### VS Code Integration

1. **Install VS Code:**
   - If you don't have VS Code installed, download and install it from the [official website](https://code.visualstudio.com/).

2. **Install Git Extension for VS Code:**
   - Open VS Code, go to the Extensions view by clicking the Extensions icon in the Activity Bar or by pressing `Ctrl+Shift+X`.
   - Search for "GitLens", "Github Pull Request", "Git Graph" and install it.

### GitHub Repositories

#### Clone a Repository in VS Code
(From Remote to Local)
1. Open VS Code and click on the 'Source Control icon' in the Activity Bar.
2. Click on "Clone Repository".
  - What if no `Clone Repository`? Go [Here](https://github.com/zyx-0314/Github-Git-Guide/blob/main/git/problems.md#git-are-not-yet-installed).
3. Enter the repository URL or Login in Github and select repository
4. Choose a directory to clone the repository into.

#### Create a New Repository
(From Local to Remote )
1. Initialize a new Git repository by clicking on the Source Control icon and then "Initialize Repository".
2. Login in Github
3. Rename (optional)(default: same name as the folder)
4. When Name already exist indicated what you can do is:
  *Rename and continue* or *Clone the repo somewhere in different directory and overwrite the code with your new code*
5. Publish in Public or Private
  *Public*: Can be viewed by anybody
  *Private*: Only you can view

### GitHub Issues

- **Managing Issues in Github Browser:**
   - Navigate to your repository on GitHub.
   - Click on the "Issues" tab and then "New issue".
   - Provide a title and description for your issue, then click "Submit new issue".

- **Managing Issues in VS Code:**
   - Install the "GitHub Pull Requests" extension from the VS Code Marketplace.
   - Use the GitHub Pull Requests Side Icon, in the Issues tab view in VS Code to create, view, and manage issues directly from your editor.

### GitHub Pull Requests

1. **Creating Pull Requests:**
   - Push your changes to a new branch in your repository.
   - Navigate to the repository on GitHub and click on "Pull requests" then "New pull request".
   - Select the branches you want to merge and provide a title and description for your pull request, then click "Create pull request".

2. **Managing Pull Requests in VS Code:**
   - Install the "GitHub Pull Requests" extension from the VS Code Marketplace.
   - Use the GitHub Pull Requests Side Icon, in the Pull Request tab view in VS Code to create, review, and manage pull requests directly from your editor.

---

You have now successfully installed Git, configured it, integrated it with VS Code, and learned how to manage GitHub repositories, issues, and pull requests. For further assistance, refer to the official documentation or community forums.
