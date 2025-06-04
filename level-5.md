#Bandit Wargame Walkthrough
**Source:** [OverTheWire – Bandit](https://overthewire.org/wargames/bandit/)

---

## Level 5 ➡️ Level 6

**Goal**:  
The password is stored in a file somewhere under the inhere directory and has all of the following properties:

Human-readable

1033 bytes in size

Not executable

**Question**:  
How do you find a file with specific properties?

**Answer**:
```bash
find inhere/ -type f -size 1033c ! -executable
cat <found_file>
```

**Explanation**:
find searches for files (-type f) of size 1033 bytes (-size 1033c) that are not executable (! -executable).
