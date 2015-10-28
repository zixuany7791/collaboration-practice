# Collaboration Practice
## _Practicing Merges & Conflicts_

---

## Task 0: Setting Up

1. Partner up. The directions for this repo are meant for two people.  If there is a third person, just rotate drivers/navigators.
2. Notice the files in this repo:  
  a. **README.md**: these directions _(do not alter this file)_  
  b. **line-numbers.md**: where you will practice!
3. Decide on ONE person to fork this repo. You are the owner.  From now on, you will be referred to as the **owner**.  Go ahead and fork this repo.
4. **Owner**: Settings (gear icon) > Collaborators > type your partner's username and "Add Collaborator".  From now on, they will be referred to as the **collaborator**.
5. **Collaborator**: check your email.  You should receive an email that contains a link to this remote repo and a message saying "You can now push to this repository."  Open the link.
6. **Both partners**: copy the `SSH URL`. In your IDE, make sure you are in `~/workspace` and then `git clone URL`.  Then `cd` into `collaboration-test`.
7. The best way to do this activity is to open up:  
  a. the **Preview** of `README.md` _(but you don't need the raw markdown)_  
  b. the **raw markdown** of `line-numbers.md` _(but you don't need the preview)_  

---

## Task 1: Automatic merges _(no errors)_

1. **Owner**: add text to line 1 (after 1).  
_ex:_ `1 Mr. Mueller wuz here!`  
2. **Collaborator**: add text to line 3 (NOT line 2).  
_ex:_ `2 Mr. Shmueller wuz here!`  
### IMPORTANT SIDENOTE:  There must be one extra line BETWEEN the edits.  Otherwise, you will get a merge conflict.
3. **Owner**: `add`, `commit`, and `push`.  You shouldn't have any issues.
4. **Collaborator**: Try to do `git pull`.  You will be prompted with an error that ends with: 
```
Please, commit your changes or stash them before you can merge. 
Aborting.  
```  
  a.  So following the directions, you must `add` and `commit`. Go ahead and do that.  
  b.  Well you're in the habit of doing `add`, `commit`, and `push`, so go ahead and try `push`ing. You should see an error:
```
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
```
  c. So you have to do `git pull`.  Then press `^X` (control X) to skip adding a "merge message". You should see the changes merged automatically!  
  d. A quick `git status` will show you that you still need to `push`.  Do that.
5. **Owner**: do a `git pull` to see your collaborator's changes as well!
6. Let's practice again, but this time in the other direction:  
  a. This time, **collaborator**: add some text to line 5, then `add`/`commit`/`push`.  
  b. And **owner**, you add text to line 7.  
  c. Repeat the same process as above, but this time so that the **owner** has to `pull`.  
7. By the end of this Task, both partners should have the same text on lines 1/3/5/7, and a `git status` (for both partners) should say:

```
On branch master
Your branch is up-to-date with 'origin/master'.

nothing to commit, working directory clean
```  

---

