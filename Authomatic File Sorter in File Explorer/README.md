
---

## 📌 Features

- Automatically detects file types: `.csv`, `.jpg`, `.txt`
- Creates folders if they don’t exist
- Moves each file to the correct folder
- Easy to extend (e.g., add support for `.pdf`, `.xlsx`, etc.)

---

## 🧠 How It Works

1. Specify the folder path containing your unsorted files
2. The script lists all files using `os.listdir()`
3. Based on file extensions:
   - `.csv` → `csv files/`
   - `.jpg` → `images/`
   - `.txt` → `text files/`
4. Files are moved using `shutil.move()`

---

## 📄 Requirements

No external libraries are needed:
- Python 3.x
- Built-in `os` and `shutil` modules

---

## 🚀 How to Run

1. Change the `path` variable to the folder you want to sort
2. Run the script in any Python environment (e.g., Jupyter Notebook)
3. Watch as your files are sorted automatically!

---

## 🔧 Customization

You can easily add more file types. For example:

```python
elif ".pdf" in file:
    shutil.move(path + file, path + "pdf files/" + file)
