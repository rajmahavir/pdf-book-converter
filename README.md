# 📚 PDF Book Format Converter

A web-based tool to convert PDFs into book format: first page solo, then paired spreads (pages 2-3, 4-5, 6-7...).

Perfect for creating digital books with proper page spreads for viewing on tablets, e-readers, or large monitors.

## ✨ Features

- **Single HTML File** - Everything embedded in one file, no installation required
- **100% Client-Side** - All processing happens in your browser, complete privacy
- **No Server Needed** - Just open the HTML file and start converting
- **Drag & Drop** - Easy file upload with drag and drop support
- **Live Preview** - Navigate through converted pages before downloading
- **Any Page Size** - Works with A4, A5, A3, or any PDF page size
- **Modern UI** - Beautiful, responsive design

## 🚀 Quick Start (EASIEST - Standalone Version)

### Just 3 Steps:

1. **Download** `pdf-converter-standalone.html`
2. **Open** it in any modern browser (Chrome, Firefox, Edge, Safari)
3. **Upload & Convert** your PDF - that's it!

**No installation. No dependencies. No server. No Python. No Node.js.**

---

## 🔧 Alternative: Backend Version (Optional)

### Step 1: Install Dependencies

**Windows:**
```bash
pip install -r requirements.txt
```

**Mac/Linux:**
```bash
pip3 install -r requirements.txt
```

### Step 2: Start the Server

**Option A - Double-click:**
- Windows: Double-click `start-backend.bat`
- Mac/Linux: Double-click `start-backend.sh`

**Option B - Command line:**
```bash
python app_server.py
# or
python3 app_server.py
```

### Step 3: Access the Application

Open your browser and go to:
- Local: `http://localhost:5000`
- Network: `http://[your-ip]:5000` (shown in terminal)

### Step 4: Use the Application

1. Upload your PDF
2. Click "Process PDF"
3. Preview all pages (use Previous/Next buttons)
4. Download the converted PDF

## 📋 How It Works

**Input:** Regular PDF with sequential pages (1, 2, 3, 4, 5, 6...)

**Output:** Book format PDF:
- Page 1: Solo (first page)
- Page 2: Spread of pages 2-3 side by side
- Page 3: Spread of pages 4-5 side by side
- Page 4: Spread of pages 6-7 side by side
- And so on...

If there's an odd number of pages, the last page will be added solo.

## 🔧 Technical Details

### Technologies Used
- **HTML5/CSS3** - Modern, responsive interface
- **JavaScript** - Frontend interaction
- **Python Flask** - Backend server
- **PyPDF2** - Reliable PDF manipulation
- **PDF.js** - PDF preview rendering

### System Requirements
- Python 3.7+ (check with `python --version`)
- Modern web browser
- Internet connection (for initial library downloads only)

### Browser Compatibility
- Chrome/Edge (Recommended)
- Firefox
- Safari
- Any modern browser with JavaScript enabled

## 📁 Project Structure

```
pdf-book-converter/
├── BACKEND VERSION (RECOMMENDED):
│   ├── index_backend.html      # Main web interface
│   ├── app_backend.js          # Frontend JavaScript
│   ├── app_server.py           # Flask server with API
│   ├── pdf_processor.py        # PDF processing logic
│   ├── requirements.txt        # Python dependencies
│   ├── start-backend.bat       # Windows startup
│   └── start-backend.sh        # Mac/Linux startup
│
├── SIMPLE VERSION (for testing/demo):
│   ├── index.html              # Client-side interface
│   ├── app.js                  # Browser-based processing
│   ├── server.py               # Simple HTTP server
│   └── start-server.bat/.sh    # Simple launchers
│
└── README.md                   # This file
```

**Use the BACKEND VERSION** for production use - it's more reliable and handles all PDF types correctly.

## 🌐 Accessing from Other Devices

1. **Start the server** on your main computer using `start-backend.bat` or `start-backend.sh`
2. **Note your IP address** (displayed when server starts, e.g., `http://192.168.1.100:5000`)
3. **On other devices** (phone, tablet, other computers):
   - Connect to same WiFi/LAN network
   - Open browser and go to the Network URL
   - Upload and process PDFs normally!

### Finding Your IP Address Manually

**Windows:**
```bash
ipconfig
```
Look for "IPv4 Address"

**Mac/Linux:**
```bash
ifconfig
```
or
```bash
ip addr show
```
Look for an address like `192.168.x.x`

## 🔒 Privacy & Security

- **All processing happens in your browser** - files never leave your device
- **No data collection** - no tracking, no analytics, no server uploads
- **Open source** - inspect the code yourself
- **LAN only** - not exposed to the internet (unless you configure port forwarding)

## 🛠️ Troubleshooting

### Installation Issues
- **"pip not found":** Make sure Python is installed and added to PATH
- **Permission errors:** On Mac/Linux, use `pip3 install --user -r requirements.txt`
- **Module not found:** Make sure you ran `pip install -r requirements.txt` first

### Server Issues
- **Port already in use:** Try a different port
  ```bash
  python app_server.py 3000
  ```
- **Permission denied:** On Linux/Mac, use ports above 1024 or run with sudo
- **Flask not found:** Run `pip install -r requirements.txt` again

### Can't access from other devices
- **Firewall blocking:** Allow Python through your firewall
- **Wrong IP:** Use the "Network" URL shown when server starts, not 127.0.0.1
- **Different network:** All devices must be on same WiFi/LAN

### PDF processing fails
- **Check server console:** Error messages will appear in the terminal
- **File corrupted:** Try opening the PDF in another viewer first
- **Encrypted PDF:** Password-protected PDFs are not supported

### Preview not showing
- **PDF.js loading:** Check your internet connection (first load only)
- **Navigation buttons missing:** They only appear for multi-page PDFs
- **Blank preview:** Check browser console (F12) for errors

## 📁 Project Structure

```
pdf-book-converter/
├── index.html          # Main web interface
├── app.js              # PDF processing logic
├── server.py           # Python HTTP server
├── server.js           # Node.js HTTP server
└── README.md           # This file
```

## 🎯 Use Cases

- **E-book Reading** - Better viewing experience on tablets
- **Digital Magazines** - Proper two-page spread layout
- **Photo Albums** - Side-by-side photo viewing
- **Comic Books** - Traditional comic book reading experience
- **Reports/Documents** - Professional two-page layout for presentations

## 🚫 Limitations

- Very large PDFs (100+ MB) may be slow to process in browser
- Some complex PDFs with forms or annotations may not convert perfectly
- Encrypted/password-protected PDFs are not supported

## 📝 License

Free to use, modify, and distribute. No warranties provided.

## 🤝 Contributing

Feel free to modify and improve this tool for your needs!

## 📧 Questions?

- Check the troubleshooting section above
- Inspect browser console (F12) for errors
- Verify your PDF isn't corrupted

---

**Enjoy your book-formatted PDFs! 📖**
