# Notes about Commits

## Here's a tiny bit of info on GitHub's commit history:

Above your fork's files, you'll see a toolbar like this.

![](../../.gitbook/assets/image.png)

**This branch is x commits ahead** shows how many commits you've made since you last interacted with my repo \(by pull request or fork\). Note that it's not the number of files you've changed \(unless you've changed each file individually, only once\), but rather how many times you've hit the **Commit** button.

**This branch is y commits behind** shows how many commits you've missed from my branch since you last interacted with my repo \(by pull request or fork\). This number will go up with each commit I make to my repo, as well as by **two or more** with every pull request that is accepted on the main repository. 

Let's explain this a little better: let's say that there's three people involved in this scenario.

* You and Person C forked my repository.
* You and Person C both make changes to some pages in the wiki.
* I commit 4 changes to my repository.
* Person C finishes 6 commits before you do and opens a pull request.
* You commit 3 changes but haven't yet opened a pull request.
* I review the pull request by Person C and deem it acceptable, and merge the changes.
* Your toolbar will read **11 commits** behind Doregon:master.
  * 6 commits from Person C
  * 4 commits from me
  * 1 commit saying "Merged `PersonC:master` into `Doregon:master`"

Sometimes, being behind on commits **can cause frustration**, especially if you edit a file only to find that it conflicts with another change made by someone else.

If you're behind, then an answer is available for you. In that toolbar, hit **Compare**. It will show you all of the differences between the commits pending to be merged on your files and the ones already changed on my repository.

Your file will always be listed \(because it differs from the original repository's\), but check the writing in it.

**If it turns out that nothing changed on the original**, you can proceed.

**If it turns out that whatever changed on the original doesn't affect your edits** \(such as adding a new line\), you can proceed with caution. GitHub might say it's conflicting because of what lines the text is on, and how you don't have those lines. You can try copying and pasting between the two files to get it exactly right if something doesn't work.

**If it turns out that whatever changed on the original does affect your edits** \(such as you overwrote a couple of lines, commit your changes, but then you find that the original doesn't have the lines that where deleted in the first place\), you can't proceed easily. However, you can make your edits work by doing the following:

1. Download your copy of the conflicting file.
2. Do one of the following:
   1. **If it's a document**, copy the original file's contents and then paste them into a new file with the same name in the same location.
   2. **If it's media**, download the file directly from the original repository.
3. Now, make your edits again while using the original as a base. **Don't** just upload the original file again, this will overwrite the original repository's edits.
4. **If that doesn't work**, try deleting and re-forking your version of the repository, and then remaking your edits.

Doing this will ensure that you we can automatically merge your pull request.

