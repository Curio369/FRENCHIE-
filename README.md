# 🇫🇷 Flashy — French Flashcard Learning App

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Tkinter](https://img.shields.io/badge/Tkinter-GUI-FF6F00?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data-150458?style=for-the-badge&logo=pandas&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

**A sleek desktop flashcard app to learn the top 100 French words — with smart progress tracking that picks up right where you left off.**

</div>

---

## 📸 Screenshots

<div align="center">

| 🇫🇷 French Side | 🇬🇧 English Side |
|:-:|:-:|
| ![French Card](img/Sample_french_img.png) | ![English Card](img/Sample_English_img.png) |
| *Card shows the French word* | *Flips automatically after 3 seconds* |

</div>

---

## ✨ How It Works

1. **A French word appears** on a white card
2. **Wait 3 seconds** — the card flips to reveal the English translation on a green card
3. **Mark yourself:**
   - ✅ **Know it?** Hit the green checkmark — the word is removed from your deck forever
   - ❌ **Don't know it?** Hit the red cross — it stays in the deck to practice again
4. **Progress is saved automatically** — next time you launch, only unseen words appear

---

## 🚀 Features

- 🔄 **Auto-flip cards** after 3 seconds with a smooth language transition
- 🧠 **Smart progress tracking** — known words are removed and saved to `words_to_learn.csv`
- 📂 **Persistent learning** — resumes from your last session automatically
- 🎨 **Clean, minimal UI** built with Tkinter and custom card images
- 📊 **100 most common French words** included out of the box

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.8+ | Core language |
| Tkinter | Desktop GUI framework |
| Pandas | CSV reading & progress saving |

---

## 📁 Project Structure

```
flashy/
├── main.py                  # Main application
├── data/
│   ├── french_words.csv     # Full word bank (100 French-English pairs)
│   └── words_to_learn.csv   # Auto-generated: your remaining words
├── images/
│   ├── card_front.png       # White card (French side)
│   ├── card_back.png        # Green card (English side)
│   ├── right.png            # ✅ Known button
│   └── wrong.png            # ❌ Unknown button
└── img/
    ├── Sample_french_img.png
    └── Sample_English_img.png
```

---

## ⚡ Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/flashy.git
cd flashy
```

### 2. Install dependencies

```bash
pip install pandas
```

> Tkinter comes built-in with Python. No extra install needed.

### 3. Run the app

```bash
python main.py
```

---

## 🔁 Progress Reset

To start over from all 100 words, simply delete the auto-generated file:

```bash
rm data/words_to_learn.csv
```

The app will fall back to the full `french_words.csv` word bank on next launch.

---

## 🗂️ Word Bank Preview

The app ships with the **100 most common French words**, including:

| French | English |
|--------|---------|
| partie | part |
| histoire | history |
| chercher | search |
| seulement | only |
| ... | ... |

---

## 🔒 Notes

- `words_to_learn.csv` is **auto-generated** at runtime — add it to `.gitignore` so your personal progress isn't committed.

```gitignore
data/words_to_learn.csv
__pycache__/
*.pyc
```

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

<div align="center">
Made with ❤️ to make French learning a little less <i>difficile</i>
</div>
