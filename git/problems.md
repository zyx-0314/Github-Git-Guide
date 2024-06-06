<a name="readme-top"/>

<br/>

<br />
<div align="center">
  <h3 align="center">Problems you may encounter</h3>
</div>

<br />

---

<br />
<br />

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#live-server-not-working">Live Server is not working</a>
      <ol>
        <li>
          <a href="#working-in-workspace-or-github">When there is [Github] or (Workspace) in your VS Code</a>
        </li>
      </ol>
    </li>
    <li>
      <a href="#no-clone-repository-button">No Clone Repository Button</a>
      <ol>
        <li>
          <a href="#occupied-work-directory">Occupied Work Directory</a>
        </li>
        <li>
          <a href="#git-are-not-yet-installed">Git are not yet Installed</a>
        </li>
        <li>
          <a href="#working-with-other-git">Working with other git</a>
        </li>
      </ol>
    </li>
  </ol>
</details>

---

## Live Server Not Working
Live server might not work in some instances and as follows are enountered, reported and solution has been found.

### Working in Workspace or Github
Reason: 
- Could be using `Remote Explorer` to access the github repository

Solution:
1. Open New Window (File > New Window or 'ctrl + shift + n')
2. Then [Clone](https://github.com/zyx-0314/Github-Git-Guide/blob/main/git/settingup-git-windows.md#github-repositories)

---

<br />

## No Clone Repository Button
Some Instances the clone repository button may not appear.

### Occupied Work Directory
This happen when you open or working with different project, working with same project but no relationship. What button/s that might appear are "Initialize Git" or "Publish Git".

1. Open New Window (File > New Window or 'ctrl + shift + n')
2. Then try to check again

### Git are not yet Installed
This happen when git is not yet installed. What button that might appear are "Download Git".

1. Follow the ["Installation" Section](https://github.com/zyx-0314/Github-Git-Guide/blob/main/git/settingup-git-windows.md#installation)

### Working with other git
This happen when you are working with different project and it has git. What button that might appear are "Commit", "Commit & Push", "Sync" or "Push".

1. Open New Window (File > New Window or 'ctrl + shift + n')
2. Then try to check again

## Missing Update Code from Othe Devices
There is a lot of reason why it might occur.

### Forget to Save, Commit and Push
If you forget to save and commit in the device where you modify code it will stay there.
And last part is the push, the button that has name of sync, it will not sync with your remote repository

### Didn't Pull
Pull is a process where you sync your current pc on the update made on repo from other devices.
Pull can be triggered by going to 'Source Control' then a 'Sync Button' is there present.