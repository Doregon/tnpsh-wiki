# Contribution Guidelines

## If you're going to make changes, you need to know some stuff.

We've spent a lot of time working, proofreading, and automating to make this wiki accurate and precise. We're setting up guidelines to show what you can and can't do with your additions and edits, and point you in the right direction.

### 1. Accuracy

We want to keep everything in the wiki as clean and typo-free as possible. That's why the **Spellcheck** Action runs every time you open a new pull request to make a change to the wiki. The Spellchecker looks in an English dictionary, as well as a predefined list of words in two texts files stored in the ".github/workflows" folder.

If you pass the spellcheck operation, you're all set and good to go! However, if you fail, try this:

1. If you haven't already, proofread your writing. You can also view the Action status by clicking on the X in the Merge box and selecting "Details."
2. If all of your words are correct but they are still being seen as incorrect, find out what words they are, make a list, and then send that list as a comment on the pull request. This will make it so that I can merge your edits by adding the words to the dictionary. Once I comment back saying it's done, try adding a random commit somewhere \(add a space at the end of a line\) to trigger the action to run again.
3. Removing this folder and its contents will render your pull request invalid.

### 2. Editable Files

Certain files aren’t allowed to be edited, unless specific permission is granted or, in some cases, you are a moderator. The following will occur depending on the situation:

1. **Items that cannot be modified**

You can’t delete, move, or edit the following files.

* .gitbook.yaml
* .github/workflows/action.yaml
* .spellcheck.yaml
* LICENSE
* about-the-wiki/acknowledgments.md

If these files are edited and a pull request is made, the pull request will be rejected.

1. **Items that cannot be modified, unless replaced.**

You can’t delete, move, or edit these files unless you have a replacement and you verify everything still works together.

* any item in the .gitbook/assets directory

**NOTE**: Don’t organize any assets into folders. The best we can do is rename each asset to a descriptive name, but using folders can get screwed up once GitBook pushes a new commit.

