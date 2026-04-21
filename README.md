# Automated-Data-Shield

## 🚀 Overview
**Automated Data Shield** is a Python-based periodic backup system designed for efficient data protection. Unlike traditional backup tools, it acts as an **incremental backup system**, intelligently copying only new or modified files by comparing their content hashes.

## ✨ Key Features
* **Smart Incremental Backup:** Uses MD5 hashing to detect changes, avoiding redundant file copies to save time and storage.
* **Automated Scheduling:** Executes backup cycles at fixed intervals using the `schedule` library.
* **Recursive Archiving:** Walks through source folders recursively and maintains the original folder structure.
* **Timestamped Compression:** Automatically creates ZIP archives with names like `Backup_2026-02-09_22-15-10.zip`.
* **Metadata Preservation:** Uses `shutil.copy2()` to ensure file metadata like timestamps are preserved

## 🛠 Tech Stack
* **Language:** Python 
* **Core Modules:** `hashlib` (MD5), `shutil` (File Ops), `os` (Pathing), `zipfile` (Compression)
* **Scheduling:** `schedule` library 
