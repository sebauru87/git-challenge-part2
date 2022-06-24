# Git challenge

## Part 2

In this lesson we've seen how to undo changes / commits so we will now do some exercises to test these new skills.

1.  Fork this [repository](https://github.com/djabif/git-challenge-part2)

2.  Create a new branch "feature-a"

    a. Create a commit updating the user's personal data with your own data. `(commit 1)`

    b. Create another commit updating the text of the footer. `(commit 2)`

    c. Undo your last commit. What command would you use and why?

    ```bash
    $ git reset --hard HEAD~1
    ```

    d. Push your changes.

3.  a. Change anything from index.html and commit. `(commit 3)`

    b. Change another thing from index.html and commit. `(commit 4)`

    c. You have realized that you introduced a bug with your `commit 1` so you want to undo the entire commit. What command would you use and why?

    ```bash
    $ git revert HEAD~2
    or
    $ git revert "hashOfTheCommit"
    ```

4.  a. Change anything from index.html and commit. `(commit 5)`

    b. After examining your previous commit, you realized you made a typo in one word so you want to undo your last commit without losing the changes, fix the typo and re commit. What command would you use and why?

    ```bash
    $ git reset --soft HEAD~1
    ```

5.  Push everything and merge your branch to main.

6.  Now you need to undo your `commit 2`. Remember that all your previous commits are now part of the `main` branch which is shared with all your coworkers so you should be aware of the command you will use here. What command would you use and why?

    ```bash
    $ git revert "hashOfTheCommit"
    ```
