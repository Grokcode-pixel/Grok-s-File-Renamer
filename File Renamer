# Grok’s File Renamer - Переименование файлов
import os

def file_renamer():
    print("Welcome to Grok’s File Renamer!")
    folder = input("Enter folder path (e.g., C:/Photos): ")
    prefix = input("Enter prefix (e.g., 'photo_'): ")
    
    if not os.path.isdir(folder):
        print("Folder not found!")
        return
    
    files = os.listdir(folder)
    for i, filename in enumerate(files, 1):
        old_path = os.path.join(folder, filename)
        new_name = f"{prefix}{i}{os.path.splitext(filename)[1]}"
        new_path = os.path.join(folder, new_name)
        os.rename(old_path, new_path)
        print(f"Renamed: {filename} → {new_name}")
    
    print(f"Done! Renamed {len(files)} files.")
    print("\nLike it? Support me: https://boosty.to/grokcode/donate")

if __name__ == "__main__":
    file_renamer()
