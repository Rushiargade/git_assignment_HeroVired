# Git Assignment – Hero Vired

This is my assignment repository for **git_assignment_HeroVired**.
I have done all the steps mentioned in the assignment. Below is what I did in simple words.

---

## Q.1 – CalculatorPlus App

1. I created a repository with the name **git_assignment_HeroVired**.

2. Made a new branch called **dev** and added the Calculator code in it.

3. The code has add, subtract, multiply and divide functions. I also implemented the **square_root** function using `math.sqrt()`.

4. Merged the dev branch into main and created **version 1 release**.

5. Added one of my classmates as a collaborator.

6. Created another branch called **feature/sqrt** and worked on square root feature there.

7. While doing this, a bug came in the divide function (divide by zero). I fixed it in **dev** branch by adding:

   ```python
   def divide(self, a, b):
       if b == 0:
           raise ValueError("Cannot divide by zero.")
       return a / b
   ```

8. After finishing the square root feature, I created a Pull Request to main branch.

9. Asked for code review, got it reviewed, and made changes.

10. Merged **feature/sqrt** into **dev**, tested, and finally merged into **main**.

11. Created **version 2 release** for CalculatorPlus app.

---

## Q.2 – Git LFS (Large File Storage)

1. Created a branch called **lfs**.
2. Installed Git LFS using commands:

   ```bash
   git lfs install
   git lfs track "*.bin"
   ```
3. Added a large file (more than 200MB) to the repository.
4. Committed and pushed it.
5. Cloned the repository on another system to check if the large file downloads correctly. It worked fine.

---

## Q.3 – Geometry Calculator

1. Created a new branch called **geometry-calculator**.
2. Wrote a class `GeometryCalculator` with two functions:

   * `calculate_circle_area(radius)`
   * `calculate_rectangle_area(length, width)`

### Workflow with Git Stash

* Made a branch **feature/circle-area**, started coding circle area but before committing, I stashed the changes.
* Then I created branch **feature/rectangle-area**, worked on rectangle area feature, and again stashed changes before committing.
* Switched back to **feature/circle-area**, applied stash, completed the code, committed and pushed.
* Went to **feature/rectangle-area**, applied stash, completed code, committed and pushed.
* Created Pull Requests for both features into **dev** branch.
* Got them reviewed and merged into **main** branch after approval.


