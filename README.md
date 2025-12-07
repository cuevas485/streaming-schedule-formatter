# 🎬 Streaming Schedule Formatter

A lightweight Python utility that converts a raw text file of streaming show releases into a clean, Discord-ready formatted embed post.

This script reads a `WhatsNew.txt` file containing shows, platforms, and release dates, then outputs a structured and stylized `.txt` file that can be directly pasted into Discord.

---

## ✨ Features
- Extracts show data using regex pattern matching  
- Converts month names into abbreviated formats (e.g., *September → Sep*)  
- Normalizes show titles (e.g., *"Season 2"* → *"S2"*)  
- Groups shows by day of the month  
- Automatically forms a clean, stylized Discord post layout  
- Auto-detects the current year if not provided  
- Includes a footer with placeholders for previous posts and sources  
- Outputs a final cleaned file:  
  **`stream_schedule_<month>_<year>_formatted.txt`**

---

## 📁 Input Format (WhatsNew.txt)

Each line must contain a timestamp, show title, platform, and date in this structure:

```
12:00 Show Title on Netflix - September 14
08:30 Another Show on Hulu - October 2
```

---

## ▶️ Usage

### 1. Place the input file
Place your `WhatsNew.txt` file in the same directory as the script.

### 2. Run the script
```
python stream_formatter.py
```

### 3. Output file
Your formatted file will be created using the pattern:

```
stream_schedule_nov_2025_formatted.txt
```

Paste this directly into Discord.

---

## 📦 Example Output

```
Monthly Stream Update
Top Streaming Shows | Nov-2025
+++

**Nov 3**
*The Witcher S3 (Netflix)*

**Nov 8**
*Loki S2 (Disney+)*

**Last Month's Post:**
[**Top Streaming Shows - October Recap**](PLACEHOLDER)

**Source**
[**Rotten Tomatoes YT**](PLACEHOLDER)
```

---

## 🧩 Dependencies
- Python 3.8+
- Standard library only

---

## 📌 Future Enhancements
- CLI flags for input/output paths  
- Support for multiple months  
- Auto-detection of previous month’s link  
- Export to Discord JSON Embed format  

---

## 📜 License
MIT License
