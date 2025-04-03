# 🗂️ Media Viewer

This is a **simple media viewer**, originally built as a small personal project. It automatically serves image, video, and text files from a `/media` directory using a clean and responsive UI.

> **Note:** This is an **older project** and may not follow the latest best practices. That said, it's still functional and **easy to expand** — perfect for learning or lightweight use cases.

---

## Features

- Auto-preview of images, videos, and text files
- Clean and minimal design
- OpenGraph metadata for link previews (Discord, Twitter, etc.)
- Direct download button
- Smart MIME type detection
- Friendly fallback redirect if file not found

---

## How It Works

1. `.htaccess` redirects all unknown file paths to `index.php` using URL rewriting.
2. `index.php` checks if the file exists inside the `/media` directory.
3. If the file exists:
    - It determines the file type
    - Renders an embedded preview (image, video, or text)
    - Adds metadata and a download button
4. If the file does **not** exist:
    - User is redirected to a fallback URL (e.g., `https://dennisamlimit.dev`)

---

## Getting Started

### Requirements
- Apache with mod_rewrite enabled
- PHP 7.0 or higher

### Installation
1. Clone or download this repository.
2. Place it inside your Apache server's root or a subdirectory.
3. Make sure the `.htaccess` file is active and the `/media` folder exists.
4. Upload any supported media file into `/media`.
5. Access it via URL:
   ```
   http://yourdomain.com/yourfile.jpg
   ```

---

## 📸 Preview

![Screenshot](screenshot.png)

---

## 📄 License

MIT License. Free to use, modify, and share.

---

## 🙋‍♂️ Author

Made with by [Dennis](https://dennisamlimit.dev)

