# Installation and Setup of WakaTime in VS Code and Displaying Stats

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
      <a href="#example">Example</a>
    </li>
  </ol>
</details>

---

## Installation

1. Sign Up for WakaTime
    - Open your web browser and navigate to [WakaTime's website](https://wakatime.com/).
    - Click on the **Sign Up** button and create an account using your preferred method (email, GitHub, or Google).
        - use **github** account for faster login/sign up.
2. Install WakaTime Extension in VS Code

    - Open **Visual Studio Code**.
    - Go to the **Extensions** view by clicking on the Extensions icon in the Activity Bar on the side of the window or by pressing `Ctrl+Shift+X`.
    - In the search box, type `WakaTime`.
    - Click on the **WakaTime** extension by WakaTime and then click **Install**.

3. Get Your WakaTime API Key
    - Go back to the WakaTime website and log in if you haven't already.
    - Option A Installation:
        - Click on your profile icon in the top right corner and select **Settings** from the dropdown menu.
        - Under the **API Key** section, copy your **API Key**.
    - Option B Installation:
        - Find and click Supported IDEs on top left panel.
        - Search for `VS Code`.
        - On Installing step 3 there is an anchor/link named `API Key` click it.
        - Copy the higlighted api key.

4. Configure WakaTime in VS Code

    - Return to **Visual Studio Code**.
    - Upon successful installation of the WakaTime extension, a pop-up will appear asking for your API Key. Paste your copied API Key into the pop-up and press Enter.
    - If the pop-up does not appear, you can manually enter the API Key by:
        - Pressing `Ctrl+Shift+P` to open the Command Palette.
        - Typing `WakaTime: API Key` and selecting the option to enter your API Key.
            - don't delete the `>`.

5. Verify WakaTime is Working

    - Start coding as usual in VS Code.
    - After a few minutes, visit your WakaTime [dashboard](https://wakatime.com/dashboard) to check if your coding activity is being tracked.

6. Display WakaTime Stats in README

    - Go to your GitHub repository where you want to display your WakaTime stats.
    - Edit your `README.md` file by clicking on the pencil icon in the top right corner.

    - Add the following Markdown code to display your WakaTime stats:
        - Note: Replace `YOUR_WAKATIME_USERNAME` with your actual WakaTime username.
        - Other Waka Time Display options can be found here, [Waka stats](https://wakatime.com/share).

    ```markdown
    ## My WakaTime Stats

    ![WakaTime stats](https://github-readme-stats.vercel.app/api/wakatime?username=YOUR_WAKATIME_USERNAME&layout=compact)
    ```

    - Commit the changes to your `README.md` file.

7. Verify the Stats in README

    - Go to your GitHub repository's main page and ensure that the WakaTime stats are displayed correctly in the `README.md` file.

## Example

Here’s an example of how the section in your `README.md` file might look:

```markdown
# My Project

Welcome to my project!

## My WakaTime Stats

![WakaTime stats](https://github-readme-stats.vercel.app/api/wakatime?username=ianramirez)

## Features
- Feature 1
- Feature 2

## Installation
Instructions on how to install the project.

## Usage
Instructions on how to use the project.
```

This setup will automatically display your coding activity tracked by WakaTime in your GitHub repository's `README.md` file.