

### **🚀 Steps to Reset Git History Using an Orphan Branch**
⚠ **Warning:** This will permanently remove all commit history. Make a backup if needed.

---

### **1️⃣ Create an Orphan Branch**
```bash
git checkout --orphan new-main
```
This creates a **new branch** with no commit history.

---

### **2️⃣ Add and Commit Files**
```bash
git add .
git commit -m "Reset: Fresh start"
```

---

### **3️⃣ Delete Old Main Branch**
```bash
git branch -D main  # If your branch is named "main"
git branch -D master  # If your branch is named "master"
```

---

### **4️⃣ Rename Orphan Branch to Main**
```bash
git branch -m main  # Rename orphan branch to 'main'
```

---

### **5️⃣ Force Push to Remote (Erase History)**
```bash
git push --force origin main
```

✅ **Done! Your repository now has a fresh start with no history.**  

