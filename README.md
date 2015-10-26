# tempo-translations
## Instructions for translators

Getting familiar with the project
Start by opening the tempo-translations project on GitHub



To see the translations for each product, look in the “product” directory. There you’ll find Tempo’s products, open the one you are interested in.

!(images/product-folders.png)


Inside each product’s directory there are directories for the various languages that Tempo supports, with country and language codes. There is also the master translation file “tempo-i18n.properties” which you don’t have to worry about. Open the folder with the language that you are interested in.
 
!(images/lang-folders.png)

Inside each of those directories are three files:
- missing-admin-tempo-i18n_xx_XX.properties
- missing-tempo-i18n_xx_XX.properties
- tempo-i18n_xx_XX.properties

Where xx_XX is the country and language code. The files are very simply structured, each line contains a “key” and a “string” with an equals sign = in between. The key never changes for the different languages but the strings are translated. The key must never be separated from the string, otherwise the Tempo products cannot parse the translation files.

The third file is the file that the translator will be working in and the only one that he or she will change. A translator is either improving an existing translation or adding new translations. Each use case has slightly different working methods.

Improving existing translations
If the translator is interested in improving the existing translation, then he or she is free to work on the third file, which contains all translated strings for the specified language. Simply change the text in the language and commit your changes to that file. See “How to work on Tempo translations” in this document on how to get started.

Adding translations
The two “missing-” files contain strings that have not yet been translated for the specified language. The strings for the admin sections in a separate file. Strings in these files are in the default language, English. If the translator is interested in adding translations for the specified language then he or she needs to copy and paste the strings that are going to be translated from the “missing-” files into the tempo-i18n_xx_XX.properties, at the end of the file.


# How to work on Tempo translations
## Getting started
Create GitHub account (if you don’t have one) and sign in.

To work on the translations you can either
1. Clone the project to your computer (see https://help.github.com/ for more details) and work on it locally
1. Work on the files directly in the browser by pressing the “Edit” button in the file you are going to work on

Whichever you pick, create a branch for new translation work with a descriptive name (example: timesheets-7.13-polish) and commit/propose changes to that branch

**Be sure to create a branch!** See screenshot below that shows the correct option for the in-browser editor.

!(images/commit-new-branch.png)

## Making changes
Now you have created a branch which you will be working in until you are done with your translation work. Be sure to make all changes to your branch, not the master branch.

When returning to the tempo-translations project later, you can find your branch on the “branches” page here: https://github.com/TempoSoftware/tempo-translations/branches

When committing/proposing a change later, *be sure to select your branch* and select "Commit directly to...", **don’t create additional branches**. See screenshot below for the correct option.

!(images/commit-directly.png)

When you are done with your translation work, you need to create a pull request. This can be done on your branches’ page on GitHub and pressing the green “Create pull request” button

!(images/create-pull-request-icon.png)

This will open up a compare page, where you can review your changes, but you have to press the big green “Create pull request” button to finalize the request.

!(images/comparing-changes.png)

After creating the pull request, Tempo staff will review the work and implement it in the product. You will get GitHub notifications when the changes are accepted, and Tempo will email you to let you know which version the translations will appear in.
