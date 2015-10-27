# Collaboration Test
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
2. **Collaborator**: add text to line 3.  
_ex:_ `2 Mr. Shmueller wuz here!`  
### SIDENOTE:  There must be one extra line BETWEEN the edits.  Otherwise, you will get a merge conflict.
3. **Owner**: `add`, `commit`, and `push`.  You shouldn't have any issues.
4. **Collaborator**: Try to do `git pull`.  You will be prompted with an error that says 
```
Please, commit your changes or stash them before you can merge. Aborting.  
```  
  a.  So following the directions, you must `add` and `commit`. Go ahead and do that.  
  b.  Well you're in the habit of doing `add`, `commit`, and `push`, so go ahead and try `push`ing. You should see an error:
```
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
```
5. 