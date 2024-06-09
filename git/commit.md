<a name="readme-top"/>

<br/>

<br />
<div align="center">
  <h3 align="center">Best Practices for Git Commit Messages</h3>
</div>

<br />

---

<br />
<br />

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#overview">Overview</a>
    </li>
    <li>
      <a href="#commit-message-format">Commit Message Format</a>
        <ol>
            <li>
                <a href="#detailed-breakdown-of-the-format">Detailed Breakdown of the Format</a>
                <ol>
                    <li>
                        <a href="#header">Header</a>
                    </li>
                    <li>
                        <a href="#body">Body</a>
                    </li>
                    <li>
                        <a href="#footer">Footer</a>
                    </li>
                </ol>
            </li>
        </ol>
    </li>
    <li>
      <a href="#commit-types-and-their-meanings">Commit Types and Their Meanings</a>
    </li>
    <li>
      <a href="#additional-commit-types">Additional Commit Types</a>
    </li>
    <li>
      <a href="#best-practices">Best Practices</a>
    </li>
    <li>
      <a href="#example-commit-messages">Example Commit Messages</a>
    </li>
  </ol>
</details>

---

## Overview

Using a standardized commit message format in Git helps in maintaining a clean, informative, and manageable project history. The format outlined here follows the **Conventional Commits** specification, which is a popular convention for writing clear and consistent commit messages.

Here’s a detailed breakdown of best practices for structuring your Git commit messages, including using the specified format and understanding different commit types like `fix`, `chore`, and `refactor`.

---

<br />

## Commit Message Format

The format `<type>[optional scope]: <description>` is widely adopted for its clarity and structure. Here's how to use it effectively:

1. **Type**: Indicates the purpose of the commit.
2. **Optional Scope**: Specifies what part of the code is affected (e.g., a specific module or component).
3. **Description**: Provides a brief, imperative description of the change.

Optional sections can include:
- **Body**: Offers additional context or details about the commit.
- **Footer**: Used for referencing issues, breaking changes, or additional notes.

---

### Detailed Breakdown of the Format

#### Header

- **Type**: Represents the category of the change.
  - Example: `fix`, `feat`, `chore`, `refactor`, etc.
- **Optional Scope**: A concise description of what part of the code is affected.
  - Example: `api`, `ui`, `auth`, etc.
- **Description**: A brief and imperative description of what the change does.
  - Use present tense and avoid punctuation at the end.
  - Example: `add user login functionality`, `fix API response time issue`.

**Format Example**:  
`fix(auth): resolve token expiry issue`

#### Body

The body is optional and can be used to provide more context about the commit. It should be concise but informative enough to understand the change without looking at the code.

**Format Example**:
```
fix(auth): resolve token expiry issue

The token expiry handling in the authentication module was causing
frequent logouts. Adjusted the token lifespan and added a refresh mechanism.
```


#### Footer

The footer is also optional and is typically used to reference issues or note breaking changes. You can also include additional notes or instructions here.

**Format Example**:
```
fix(auth): resolve token expiry issue

The token expiry handling in the authentication module was causing
frequent logouts. Adjusted the token lifespan and added a refresh mechanism.

Resolves: #123
BREAKING CHANGE: Users will need to re-authenticate post-update.
```


---

## Commit Types and Their Meanings

### 1. **fix**

- **Purpose**: To address a bug in the code.
- **Example**: Bug fixes or corrections that make the software function as intended.
- **Format Example**:  
  `fix(login): correct username validation logic`

### 2. **chore**

- **Purpose**: Refers to changes that do not impact the functionality of the code.
- **Example**: Maintenance tasks like updating dependencies, configurations, or tooling.
- **Format Example**:  
  `chore(deps): update dependency versions`

### 3. **refactor**

- **Purpose**: Indicates code changes that improve structure, readability, or performance without altering external behavior.
- **Example**: Code optimization or restructuring to improve maintainability.
- **Format Example**:  
  `refactor(ui): simplify form component structure`

---

## Additional Commit Types

While not specifically asked, understanding some other common commit types can be beneficial:

- **feat**: Introduces a new feature or functionality.
  - `feat(payment): add credit card processing module`
- **docs**: Pertains to documentation changes.
  - `docs(README): update installation instructions`
- **style**: Changes that do not affect the meaning of the code (formatting, missing semi-colons, etc.).
  - `style(lint): fix linting issues in service files`
- **test**: Adds or updates tests.
  - `test(auth): add unit tests for token generation`

---

## Best Practices

1. **Be Descriptive and Concise**: Commit messages should be informative but not overly verbose. Aim for a balance where anyone reading the history can understand the purpose of each change.
  
2. **Use Imperative Mood**: Write your commit messages as commands. For instance, "Add feature X" rather than "Added feature X".

3. **Scope**: Use the scope field to denote the part of the codebase affected by the commit, which helps in quickly understanding which area of the code the change relates to.

4. **Separate Logical Changes**: Each commit should encapsulate a single logical change. Avoid lumping multiple unrelated changes into a single commit.

5. **Include Issue References**: When possible, include references to issue trackers or ticket numbers to provide context and traceability.

6. **Utilize Footer for Additional Information**: Use the footer for things like breaking changes, issue resolutions, or special instructions.

By following these best practices, your commit messages will contribute to a clear and maintainable project history that is easier for everyone to understand and navigate.

---

## Example Commit Messages

1. **Fixing a Bug**
```
fix(api): handle null response in user endpoint

The user endpoint was returning null values, causing application crashes.
This change adds checks to ensure null responses are handled gracefully.

Resolves: #456
```

2. **Adding a New Feature**
```
feat(ui): implement dark mode toggle

Added a dark mode toggle to the user interface, allowing users to switch
between light and dark themes. This enhances the user experience.

Closes: #789
```

3. **Updating Documentation**
```
docs(api): update API usage examples in README

Updated the README file to include new examples for the updated API endpoints.
This helps users to quickly understand and integrate with the API.
```

4. **Performing a Code Refactor**
```
refactor(auth): improve token handling logic

Refactored the token handling logic in the authentication module to improve
code readability and maintainability. No functional changes were made.
```

## Additional Best Practices

### 1. **Regular Commits**
Make commits frequently to ensure changes are incremental and easier to manage. This also facilitates better collaboration and tracking of progress.

### 2. **Atomic Commits**
Ensure each commit is atomic, meaning it represents a single, logical change. This practice helps in understanding and reverting changes if necessary.

### 3. **Commit Often, Push Regularly**
Commit changes locally often and push them to the remote repository regularly to ensure your work is backed up and shared with your team.

### 4. **Avoid Commiting Generated Files**
Generated files or build outputs should not be committed. Use a `.gitignore` file to prevent these from being included in commits.

### 5. **Meaningful Commit Messages**
Avoid generic messages like "fix" or "update." Instead, describe what was fixed or updated to provide better context.

### 6. **Review Commit History**
Periodically review commit history to ensure consistency and clarity. Refactor commit messages if necessary to maintain a clean history.

By adhering to these guidelines, your commit messages will be more effective in communicating the intent and context of changes to the codebase.