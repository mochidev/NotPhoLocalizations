# Not Phở Localizations
 
This project contains translation files that you can use as a template when adding your native language. All contributions are appreciated, and will be accepted through GitHub Pull Requests.

## Getting Started
1. Create a [GitHub account](https://github.com/join).
2. Download [GitHub Desktop](https://desktop.github.com).
3. [Fork](https://github.com/mochidev/NotPhoLocalizations/fork) this project so GitHub can create a copy of this repo just for you to work with. (The Fork button is in the upper right corner of the screen.)

## How to Contribute

### Contributing Corrections or Edits

Contributing corrections and edits is easy, and can be done directly on GitHub! Please fork the project before continuing.

1. On your fork's page, Locate the `.lproj` folder for your language. In there you will see two files: `FoodItems.strings` and `Localizable.strings`.
2. Click on the `.strings` file you wish to edit to view its contents.
3. To edit it, Click on the pencil icon in the upper right corner.
4. Make your changes to the phrase on the right side of the `=`. See [How to edit and format `.strings` files](#how-to-edit-and-format-strings-files) below for more information.
5. Commit any changes at the bottom of the screen, explaining what you changed. If you don't commit, your changes won't be saved!
6. Submit a Pull Request so the changes can be reviewed. A button should be available on your fork's main page after you commit your changes.
7. Enter a title and description, and click on the button to submit your pull request.

### Contributing a new Language

Contributing a new language is a bit more involved, but is very much appreciated! Please **fork the project** and **download and run GitHub Desktop** before continuing. If this is your first time using git, you are encouraged to go through the tutorial that GitHub Desktop provides.

1. On your fork's page, clone this project by clicking the green Code button on the top right of the project page.
2. Choose **Open with GitHub Desktop** to save a copy of the project locally on your computer. It will open in GitHub Desktop so you can track changes.
3. Locate the `en.lproj` folder and duplicate it, renaming it to the language you are adding. Language codes can be found [here](https://www.ibabbleon.com/iOS-Language-Codes-ISO-639.html).
	- For example, if you are adding Spanish, then rename the folder to `es.lproj`.
	- If you are adding variations on Spanish as spoken in Mexico, then rename the folder to `es-MX.lproj`.
4. You should edit all `.strings` files in your language's `.lproj` folder. You can refer back to the `en.lproj` folder and its contents if you need examples. See [How to edit and format `.strings` files](#how-to-edit-and-format-strings-files) below for more information.
5. After saving your changes, use GitHub Desktop to commit those changes by providing a few words explaining what you changed in the Summary text field, then click the commit button underneath it.
6. Click the Publish (Sometimes seen as Push) button at the top to push any changes back to GitHub.
7. Click on Create Pull Request in GitHub Desktop, or from your fork's page (there should be a green highlighted section that appears) to submit a **Pull Request**.
8. Enter a title and description, and click on the button to submit your pull request.
	
## How to edit and format `.strings` files

In the `FoodItems.strings` file, only change text that is on the right of the `=` sign, contained within double quotes `"`.

- For example: `"carrot.Subtitle" = "Carrot";` → `"carrot.Subtitle" = "Cà Rốt";`
- For example: `"vinegar.Subtitle" = "White Vinegar";` → `"vinegar.Subtitle" = "Giấm Trắng";`

In the `Localizable.strings` file, also only change text that is on the right of the `=` sign. However, there will be some cases where you don't want to translate things, so do read the comments and leave those lines as is. Please use the english localization as reference for what to translate, and what to leave as is.

1. Any Vietnamese terminology that is wrapped in `##` should not be changed. They will appear in bold in the app.
2. Some languages are supported for VoiceOver, an accessibility feature where the a voice like Siri will read out the screen's contents to the user, so you might need to change some words around so it can read it out correctly.
	- For example:
```js
/* Banh Mi Ingredients GrilledPork Amount */
"BanhMi.Ingredients.GrilledPork.Amount" = "4-6 oz";

/* Banh Mi Ingredients GrilledPork Amount (VoiceOver) */
"BanhMi.Ingredients.GrilledPork.AccessibilityAmount" = "4 to 6 ounces";
```
3. To ensure that VoiceOver is working correctly, once your Pull Request has been accepted, we will send you a TestFlight version of the app with your localization added so you can test everything.
