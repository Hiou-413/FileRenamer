# 📁 Batch File Renamer

This project provides a simple PowerShell script and a batch file to **bulk rename files** in a selected folder by **replacing specific text** in their filenames.

---

## 📜 Files

- **rename_files.ps1**  
  A PowerShell script that:
  - Opens a folder selection dialog.
  - Asks for the text to replace and the new text.
  - Renames all matching files in the selected folder.

- **run_rename.bat** (example name)  
  A batch file that:
  - Executes the PowerShell script with the proper permissions.
  - Automatically pauses after execution to show the result.

---

## ⚙️ How to Use

1. **Download** both `rename_files.ps1` and the batch file (`run_rename.bat`) into the same folder.

2. **Run** the batch file (`run_rename.bat`).

3. In the window that appears:
   - Select the folder containing the files you want to rename.
   - Enter the text you want to replace.
   - Enter the new text.

4. The script will rename the files automatically.  
   A message "Renaming completed successfully!" will appear when done.

---

## ⚡ Notes

- **Safe**: Only files (not folders) are processed.
- **Flexible**: Works for any file types within the selected folder.
- **Requirements**:  
  Windows with PowerShell available (default for Windows 10/11).

- If you encounter execution policy errors, running through the provided batch file should bypass restrictions safely (`-ExecutionPolicy Bypass`).

---

## 📦 Example

Imagine you have files like:
holiday_photo1.jpg holiday_photo2.jpg holiday_photo3.jpg

If you replace `"holiday"` with `"vacation"`, after running the tool, they will become:

vacation_photo1.jpg vacation_photo2.jpg vacation_photo3.jpg


---

# 📜 License

This project is licensed under the [MIT License](LICENSE).
