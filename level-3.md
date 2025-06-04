#Bandit Wargame Walkthrough
**Source:** [OverTheWire – Bandit](https://overthewire.org/wargames/bandit/)

---

## Level 3 ➡️ Level 4

**Goal**:  
The password is stored in a hidden file in the inhere directory.

**Question**:  
How do you find and read hidden files in a directory?

**Answer**:
```bash
ls -la inhere
cat inhere/.hidden
```

**Explanation**:
ls -la lists all files, including hidden ones (starting with a dot). Then use cat to read it.
