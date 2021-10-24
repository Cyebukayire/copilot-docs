# Getting Started with GitHub Copilot in JetBrains 


- [Getting Started with GitHub Copilot in JetBrains](#getting-started-with-github-copilot-in-jetbrains)
  - [1. Installing the JetBrains extension](#1-installing-the-jetbrains-extension)
  - [2. Seeing your first suggestion](#2-seeing-your-first-suggestion)
  - [3. Choosing alternate suggestions](#3-choosing-alternate-suggestions)
  - [4. Getting more suggestions](#4-getting-more-suggestions)
  - [5. Generating code from a comment](#5-generating-code-from-a-comment)
  - [6. More examples](#6-more-examples)
  - [7. Keyboard shortcuts](#7-keyboard-shortcuts)
  - [8. Enabling and disabling GitHub Copilot](#8-enabling-and-disabling-github-copilot)
  - [9. Learn More](#9-learn-more)

<a name="1-installing-the-jetbrains-extension"></a>
## 1. Installing the JetBrains extension

1. From the JetBrains marketplace, search for 'github copilot'.  (You must include the 'github' to avoid other plug-ins with similar names.)

   <img src='resources\search-for-github-copilot_jetbrains.png' width="600px" alt="Search for `github copilot`"/>

2. Click the 'Install' button.
3. Accept the Third-Party Plugins Privacy Notice.
4. Exit and restart the IDE.

5. In the Tools menu you will now see a GitHub Copilot option.

   <img src='resources\sign-in_jetbrains.png' width="600px" alt="Tools GitHub Copilot option`"/>
  
6. Login to GitHub Copilot using the device auth flow and authorized GitHub Copilot IntelliJ plugin with your GitHub Account in an external browser.
7. Read and agree to the GitHub Copilot additional telemetry terms.
8. Click `OK`.

   Now when you start editing, you should see GitHub Copilot suggestions.

   If you receive the following message, you have not yet been added to the GitHub Copilot Technical Preview.

   <img alt="Not in the preview" src="resources/not-in-preview_jetbrains.png" width="600"></img>

   The Technical Preview is open to a limited number of testers. To join the 
   waitlist, visit [copilot.github.com](https://copilot.github.com).

   Having problems installing? Visit the [Feedback forum](https://github.com/github/feedback/discussions/categories/copilot-feedback).

<a name="2-seeing-your-first-suggestion"></a>
## 2. Seeing your first suggestion

GitHub Copilot provides code suggestions for dozens of languages and a wide variety of frameworks, 
but it works especially well for Python, JavaScript, TypeScript, Ruby, Java, and Go. 
The following samples are in Java, but other languages will work similarly.

1. Create a new Java (.java) file.
2. Create a class by typing
```class Test ```

   Copilot will suggest a class body.

   <img alt="Class code suggested by GitHub Copilot" src="resources\suggestion-class_jetbrains.png" width="600"></img>
   
   Press `tab` to accept the suggestion.

3. Below the bracket of the `main` function, type the following function header:

   ```
   int calculateDaysBetweenDates(
   ```

3. GitHub Copilot will automatically suggest an entire function body in grayed text, as shown below. 
The exact suggestion may vary.

   <img alt="Code suggested by GitHub Copilot" src="resources\suggestion-function-body_jetbrains.png" width="600"></img>

4. Press `Tab` to accept the suggestion.

GitHub Copilot will attempt to match your code's context and style. You can edit the suggested code as you choose.

<a name="3-choosing-alternate-suggestions"></a>
## 3. Choosing alternate suggestions

For any given input, GitHub Copilot can provide multiple suggestions. 
As the developer you are always in charge; you can select which suggestion to use, or reject them all.

1. Remove the function you entered and type the following again:

   ```
   int calculateDaysBetweenDates(
   ```

2. GitHub Copilot will again show you a suggested completion.

3. Instead of pressing `Tab`:
   * On macOS, press `Option`+`]` for next or `Option`+`[`) for previous.
   * On Windows or Linux, press `Alt`+`]` for next or `Alt`+`[` for previous.

   GitHub Copilot will cycle through other alternative suggestions.

4. When you see a suggestion you like, press `Tab` to accept it.

5. If you don't like any of the suggestions, press `Esc`.

<a name="4-getting-more-suggestions"></a>
## 4. Getting more suggestions

Sometimes, you may not want to use any of the initial suggestions. 
You can ask GitHub Copilot to return more.

1. Remove the function you entered and type the following again:

   ```
   int calculateDaysBetweenDates(
   ```

2. GitHub Copilot will again show you a suggested completion.

3. Open GitHub Copilot.
   * On macOS, press `Option`+`Enter`.
   * On Windows or Linux, press `Alt`+`Enter`.

   <img alt="Open GitHub Copilot" src="resources\command-palette_jetbrains.png" width="600"></img>

   Select "Open Copilot". GitHub Copilot will open a new tab and suggest multiple options, as shown below.

   <img alt="Suggestions window" src="resources\completions-pane_jetbrains.png" width="600"></img>

4. Pick a suggestion that you want to use, then click "Accept solution."

5. If you don't like any of the returned suggestions, just close the suggestions tab.

<a name="5-generating-code-from-a-comment"></a>
## 5. Generating code from a comment

GitHub Copilot can understand significantly more context than most code assistants, 
and can generate entire functions from something as simple as a comment. 

1. Remove the function you entered and type the following:

   ```
   // find all images without alternate text
   // and give them a red border
   void process() {
   ```

2. GitHub Copilot will automatically suggest an implementation:

   <img alt="Suggestions window" src="resources\code-from-comment_jetbrains.png" width="600"></img>

<a name="6-more-examples"></a>
## 6. More examples

GitHub Copilot has even more capabilities. 
Check out the examples on [copilot.github.com](https://copilot.github.com) to see more, 
or the [Gallery](https://github.com/github/copilot-docs/tree/main/gallery) in 
this repository for the latest examples from us and the community.

Got an example of your own? We welcome you to share it on our [Feedback forum](https://github.com/github/feedback/discussions/categories/copilot-feedback).

<a name="7-keyboard-shortcuts"></a>
## 7. Keyboard shortcuts

The following lists the most common keyboard shortcuts relevant for GitHub
Copilot. If you wish to rebind them, check out [the configuration guide](configuring.md).

* Accept an inline suggestion: `Tab`.

* Dismiss an inline suggestion: `Esc`.

* Show next inline suggestion: `Alt + ]` or `Option + ]`.

* Show previous inline suggestion: `Alt + [` or `Option + [`.

* Trigger inline suggestion: `Alt + \` or `Option + \`.

* Open Copilot (up to 10 suggestions in separate pane): `Alt + Enter` or `Option + Enter` then pick "Open Copilot".

<a name="8-enabling-and-disabling-github-copilot"></a>
## 8. Enabling and disabling GitHub Copilot

You can logout (or login) from Copilot from the `Tools`/`GitHub Copilot` menu.

   <img alt="The GitHub Copilot submenu in the Tools menu" src="resources\logout_jetbrains.png" width="600"></img>

<a name="9-learn-more"></a>
## 9. Learn More

To learn more about configuring GitHub Copilot, go to the [documentation table of
contents](README.md).