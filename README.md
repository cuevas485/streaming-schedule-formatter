# Rotten Tomatoes Streaming Schedule Formatter

This repository contains a simple but powerful Jupyter Notebook (`.ipynb`) workflow that converts a raw text dump from Rotten Tomatoes’ monthly “What’s New to Streaming” YouTube video into a clean, structured, Discord‑ready formatted text file.

## 📌 Overview

Each month, Rotten Tomatoes posts a YouTube video listing upcoming streaming releases.  
This project takes your manually copied list (from the video description or transcript), stored in a file named `WhatsNew.txt`, and transforms it into a polished, organized output file that is ready to paste directly into a Discord announcement channel.

The transformation includes:
- Extracting show titles, platforms, and dates
- Normalizing dates + auto-detecting month/year
- Grouping shows by day
- Formatting output for Discord embeds
- Exporting a final file like:  
  `stream_schedule_dec_2025_formatted.txt`

## 📂 Workflow Summary

1. Copy the “What’s New” timestamps and descriptions from Rotten Tomatoes.
2. Paste them into `WhatsNew.txt`.
3. Open and run the `formatter.ipynb` Jupyter Notebook.
4. A clean, structured output file is generated automatically.
5. Paste the formatted output into your Discord server.

## 🧠 Why a Jupyter Notebook?

This project uses a **Jupyter Notebook (`.ipynb`)**, which makes it easier to:
- See formatted output step-by-step  
- Debug parsing issues  
- Tweak formatting and re-run cells interactively  
- Keep monthly formatting adjustments simple

No command-line execution is required — just open the notebook and run the cells.

## 📝 Input Format Example

Your `WhatsNew.txt` file should contain lines like:

```
00:00 The Abandons Season 1 on Netflix - December 4
01:54 Spartacus: House of Ashur Season 1 on STARZ - December 5
04:12 Percy Jackson and the Olympians Season 2 on Disney+ - December 10
```

## ✅ Output Example

```
Monthly Stream Update
Top Streaming Shows | Dec-2025
+++

**Dec 4**
*The Abandons S1 (Netflix)*

**Dec 5**
*Spartacus: House of Ashur S1 (STARZ)*
```

## 📦 Output File

The notebook automatically generates:

```
stream_schedule_<month>_<year>_formatted.txt
```

Example:

```
stream_schedule_dec_2025_formatted.txt
```

## 🛠 Requirements

- Python 3.8+
- Jupyter Notebook
- No external libraries required — only Python standard library

## ▶️ How to Run

1. Launch Jupyter Notebook:
   ```
   jupyter notebook
   ```
2. Open `formatter.ipynb`
3. Run all cells
4. Check the output folder for the generated file

---

## 📌 Future Enhancements
- CLI flags for input/output paths  
- Support for multiple months  
- Auto-detection of previous month’s link  
- Export to Discord JSON Embed format  

---

## 📜 License
This project is free to use, modify, and share.
