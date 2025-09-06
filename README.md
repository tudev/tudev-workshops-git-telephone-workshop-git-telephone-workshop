# 📚 TUDev Git Telephone Workshop

Welcome to the **TUDev Git Telephone Workshop**! 🎉

In this activity, we’ll learn Git basics by playing a fun spin on the classic **telephone game**. Instead of whispering a phrase, we’ll pass it along through **commits and branches**. By the end, we’ll merge everything together into one (probably hilarious) final sentence.

---

## 🛠 What You’ll Learn

- How to **clone** a repository
- How to **branch** and work in parallel
- How to **commit** changes
- How to **push and pull** from GitHub
- How to **merge branches** and resolve conflicts

---

## 📂 Starter Files

- `story.txt` → contains the starting sentence:
  ```
  TUDev is awesome!
  ```
- `README.md` → this file (instructions).

---

## 🚀 Getting Started

1. **Clone your team repo**

   ```bash
   git clone <your-team-repo-url>
   cd git-telephone
   ```

2. **Create a branch with your name**

   ```bash
   git checkout -b edit-yourname
   git push -u origin edit-yourname
   ```

3. **Make your edit**

   - Open `story.txt`
   - Change the sentence slightly (like in the telephone game).

4. **Commit your change**

   ```bash
   git add story.txt
   git commit -m "Changed story to: TUDev hosts pizza robots!"
   git push
   ```

5. **Pass it to the next teammate**
   - The next teammate pulls and repeats:
     ```bash
     git pull origin edit-theirname
     ```

---

## 🔀 Merging in Your Team

Once everyone has made their edits:

1. One teammate (the “merger”) switches to `main`:

   ```bash
   git checkout main
   git pull origin main
   ```

2. Merge each teammate’s branch into `main`:

   ```bash
   git merge edit-yourname
   git merge edit-teammate
   git push origin main
   ```

3. If there’s a **conflict**, open `story.txt`, resolve the conflict, then:
   ```bash
   git add story.txt
   git commit
   git push
   ```

---

## 🎉 The Grand Finale

At the end, TUDev will merge all team repos into one **final story**. We’ll read it aloud together to see how the message transformed.

---

## 📘 Resources

- [Git Documentation](https://git-scm.com/doc)
- [Learn Git Branching Game](https://learngitbranching.js.org/)
- [GitHub Classroom Docs](https://classroom.github.com/)

---

✨ Have fun and don’t worry if you hit a conflict — that’s part of the game!
