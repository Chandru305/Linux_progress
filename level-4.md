#Bandit Wargame Walkthrough
**Source:** [OverTheWire – Bandit](https://overthewire.org/wargames/bandit/)

---

## Level 4 ➡️ Level 5

**Goal**:  
The password is stored in the only human-readable file in the inhere directory.

**Question**:  
How can you find a human-readable file among many?

**Answer**:
```bash
file inhere/* #Look for the file that says ASCII text.
cat inhere/<that_filename>
```

**Explanation**:
The file command tells you the type of each file. You're looking for plain text (ASCII) — not binary.
