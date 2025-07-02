---

## 🧠 How to Install Cursor AI on Ubuntu

> 💡 **Cursor** is an AI-powered coding editor. This guide helps you install it on Ubuntu and launch it from the terminal using the command `cursor`, just like you do with `code` for VS Code.

---

### 📥 1. Download the AppImage

Go to [https://www.cursor.sh](https://www.cursor.sh) and download the latest `.AppImage` for Linux.

You’ll get a file like:

```
Cursor-1.1.7-x86_64.AppImage
```

---

### 📦 2. Move It to a Permanent Location

Let’s move it to a system-wide location:

```bash
sudo mkdir -p /opt/cursor
sudo mv ~/Downloads/Cursor-1.1.7-x86_64.AppImage /opt/cursor/cursor.AppImage
sudo chmod +x /opt/cursor/cursor.AppImage
```

---

### 🔗 3. Create a Terminal Command (`cursor`)

To run Cursor from anywhere in your terminal:

```bash
# First remove any existing or broken command
sudo rm -f /usr/local/bin/cursor

# Then create the new link
sudo ln -s /opt/cursor/cursor.AppImage /usr/local/bin/cursor
```

Now you can simply launch it by typing:

```bash
cursor
```

🎉 That’s it! No desktop integration, no bloat — pure terminal power.

---

### ✅ You're Done!

* ✅ Cursor is installed
* ✅ Run it from anywhere using: `cursor`
* 🧠 Feels just like using `code` for VS Code

---

> *If you ever update Cursor, just replace the AppImage at `/opt/cursor/cursor.AppImage` and you're good to go!*

---

