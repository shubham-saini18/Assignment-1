# 🐧 Linux & DevOps Practice Assignment

> **Author:** Shubham Saini  
> **Date:** 2025-08-13

This assignment covers essential Linux and DevOps tasks to help you build a strong foundation in file management, permissions, environment variables, and basic CLI operations.

---

## 📑 Table of Contents

1. [Creating and Renaming Files/Directories](#1-creating-and-renaming-filesdirectories)
2. [Viewing File Contents](#2-viewing-file-contents)
3. [Searching for Patterns](#3-searching-for-patterns)
4. [Zipping and Unzipping](#4-zipping-and-unzipping)
5. [Downloading Files](#5-downloading-files)
6. [Changing Permissions](#6-changing-permissions)
7. [Working with Environment Variables](#7-working-with-environment-variables)
8. [Notes](#notes)
9. [Outcome](#outcome)

---

## 1. Creating and Renaming Files/Directories

**Create a Directory:**
```bash
mkdir test_dir
```
_Makes a new folder named `test_dir`._

**Create an Empty File:**
```bash
touch test_dir/example.txt
```
_Creates an empty file named `example.txt` inside `test_dir`._

**Rename the File:**
```bash
mv test_dir/example.txt test_dir/renamed_example.txt
```
_Renames `example.txt` to `renamed_example.txt` in the same folder._

---

## 2. Viewing File Contents

**View the Whole File:**
```bash
cat /etc/passwd
```
_Shows the complete contents of `/etc/passwd`._

**View First 5 Lines:**
```bash
head -n 5 /etc/passwd
```
_Shows only the first 5 lines of `/etc/passwd`._

**View Last 5 Lines:**
```bash
tail -n 5 /etc/passwd
```
_Shows only the last 5 lines of `/etc/passwd`._

---

## 3. Searching for Patterns

**Find "root" in File:**
```bash
grep "root" /etc/passwd
```
_Finds all lines in `/etc/passwd` that contain the word "root"._

---

## 4. Zipping and Unzipping

**Zip a Folder:**
```bash
zip -r test_dir.zip test_dir
```
_Compresses the `test_dir` folder into `test_dir.zip`._

**Unzip into a Folder:**
```bash
unzip test_dir.zip -d unzipped_dir
```
_Extracts `test_dir.zip` into a folder called `unzipped_dir`._

**Alternative (if zip is not installed):**

_Compress:_
```bash
tar -czvf test_dir.tar.gz test_dir
```
_Creates a compressed `.tar.gz` file of `test_dir`._

_Extract:_
```bash
tar -xzvf test_dir.tar.gz -C unzipped_dir
```
_Extracts the `.tar.gz` file into `unzipped_dir`._

---

## 5. Downloading Files

**Download from URL:**
```bash
wget https://example.com/sample.txt
```
_Downloads a file from the given URL and saves it locally._

---

## 6. Changing Permissions

**Create a File:**
```bash
touch secure.txt
```
_Creates an empty file named `secure.txt`._

**Make File Read-Only:**
```bash
chmod 444 secure.txt
```
_Sets the file so everyone can only read it._

---

## 7. Working with Environment Variables

**Create a Variable:**
```bash
export MY_VAR="Hello, Linux!"
```
_Creates an environment variable named `MY_VAR`._

**View the Variable:**
```bash
echo $MY_VAR
```
_Displays the value stored in `MY_VAR`._

---

## Notes

- This assignment is for **practice and learning**.
- Commands have been tested on standard Linux distributions (Ubuntu, CentOS, Alpine).
- Some commands may require installing extra packages.

---

## Outcome

By completing this assignment, you will be confident with:

- File and directory management
- Viewing and searching content
- Compression and extraction
- Downloading files via CLI
- Permissions handling
- Environment variable usage

---
