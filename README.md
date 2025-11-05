# 📚 PDF Book Format Converter

A standalone web tool to convert PDFs into book format: first page solo, then paired spreads (pages 2-3, 4-5, 6-7...).

Perfect for creating digital books with proper page spreads for viewing on tablets, e-readers, or large monitors.

## ✨ Features

- **Single HTML File** - Everything embedded in one file, no installation required
- **100% Client-Side** - All processing happens in your browser, complete privacy
- **No Server Needed** - Just open the HTML file and start converting
- **Drag & Drop** - Easy file upload with drag and drop support
- **Live Preview** - Navigate through converted pages before downloading
- **Any Page Size** - Works with A4, A5, A3, or any PDF page size
- **Modern UI** - Beautiful, responsive design

## 🚀 Quick Start

### Just 3 Steps:

1. **Download** `pdf-converter-standalone.html`
2. **Open** it in any modern browser (Chrome, Firefox, Edge, Safari)
3. **Upload & Convert** your PDF - that's it!

**No installation. No dependencies. No server. No Python. No Node.js.**

### How to Use

1. Open `pdf-converter-standalone.html` in your browser
2. Upload your PDF using drag & drop or file picker
3. Click "Process PDF"
4. Preview all pages (use Previous/Next buttons)
5. Download the converted PDF

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
- **JavaScript** - Client-side PDF processing
- **PDF-lib** - PDF manipulation library
- **PDF.js** - PDF preview rendering

### System Requirements
- Modern web browser with JavaScript enabled
- Internet connection (for first load only, to fetch libraries)

### Browser Compatibility
- Chrome/Edge (Recommended)
- Firefox
- Safari
- Any modern browser with JavaScript enabled

## 📁 Project Structure

```
pdf-book-converter/
├── pdf-converter-standalone.html   # Complete standalone converter
└── README.md                       # This file
```

## 🔒 Privacy & Security

- **100% Client-Side** - All processing happens in your browser
- **No Server** - Files never leave your device
- **No Data Collection** - No tracking, no analytics, no uploads
- **Open Source** - Inspect the code yourself
- **Offline Ready** - Works without internet after first load

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

## 🛠️ Troubleshooting

- **Preview not showing:** Check your internet connection (first load only) or refresh the page
- **Processing fails:** Ensure the PDF isn't corrupted or password-protected
- **Slow performance:** Large PDFs may take time - wait for processing to complete
- **Blank pages:** Check browser console (F12) for errors

## 📝 License

Free to use, modify, and distribute. No warranties provided.

## 🤝 Contributing

Feel free to modify and improve this tool for your needs!

---

**Enjoy your book-formatted PDFs! 📖**
