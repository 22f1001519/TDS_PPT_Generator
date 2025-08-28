# Your Text, Your Style – Auto-Generate a Presentation

Turn bulk text, markdown, or prose into a fully formatted **PowerPoint presentation** that matches your chosen template’s look and feel.

🚀 **PPT Generator**   
📂 **License:** MIT  

---

## ✨ Objective

This app lets anyone generate professional PowerPoint presentations by simply pasting text and uploading their preferred template.

**You can:**
- Paste a large chunk of text (markdown, prose, or notes).  
- Optionally provide one-line guidance (e.g., *“turn into an investor pitch deck”*).  
- Enter your own **LLM API key** (OpenAI, Anthropic, Gemini, etc.).  
- Upload a **PowerPoint template or presentation** (`.pptx` or `.potx`).  
- Download a newly generated `.pptx` that applies your template’s **style, fonts, layouts, and images**.

---

## 🛠 Features

✅ Analyze and split text into **meaningful slide content** (not fixed count).  
✅ Infer and apply **style, colors, fonts, and layouts** from the uploaded template.  
✅ Reuse **images and assets** from the template.  
✅ Generate and export a new `.pptx` for direct download.  
✅ Support **any LLM provider** via user-supplied API key (never stored).  

---

## 📦 Requirements

- Node.js (>=18) or Python backend (depending on implementation)  
- PowerPoint template (`.pptx` or `.potx`)  
- An API key from your chosen LLM provider  

---

## ⚡ Setup & Usage

### 1. Clone Repository
```bash
git clone https://github.com/yourusername/your-text-your-style.git
cd your-text-your-style
```

### 2. Install Dependencies
```bash
npm install
# or if Python backend:
pip install -r requirements.txt
```

### 3. Run Locally
```bash
npm run dev
# or
uvicorn app:app --reload
```

### 4. Open in Browser
Visit: `http://localhost:3000`

---

## 🌐 How It Works (200–300 Words)

When a user pastes text, the system first parses it into semantic chunks using an LLM (with user-supplied API key). The LLM identifies **titles, bullet points, and slide sections** by analyzing structure, tone, and intent. If the user provides guidance like *“turn into an investor pitch deck”*, the model adjusts slide grouping and phrasing accordingly.  

Once the textual structure is defined, the app applies **visual elements** from the uploaded PowerPoint template. Layouts, fonts, theme colors, and placeholders are extracted directly from the `.pptx/.potx`. If images or icons exist in the template, they are reused in the new slides (rather than generating new AI images). This ensures the output matches the look and feel of the template with consistency.  

Finally, the app builds a new `.pptx` file by merging structured text with extracted layouts. This is exported and offered as a **download link**. Importantly, the LLM API key is only used client-side (never logged or stored), giving users full control.  

The design philosophy is to **separate style from content**: LLMs handle text transformation, while the presentation template dictates visual formatting. This approach enables users to transform raw notes, markdown, or documents into polished presentations—automatically, but still in their chosen style.

---

## 🎁 Optional Enhancements
- Auto-generate **speaker notes** for each slide.  
- Support **stylistic modes** (e.g., technical, investor pitch, visual-heavy).  
- Offer **slide previews** before download.  
- Provide **guidance templates** (e.g., “Sales Deck”, “Research Summary”).  
- Error handling for file size, upload failures, and API retries.  

---

## 📜 License
MIT License © 2025

---

## 🤝 Contributing
Pull requests and feature suggestions are welcome!  

---

## 🔗 Links
- [PowerPoint File Format Spec (ECMA-376)](https://learn.microsoft.com/en-us/openspecs/office_standards/ms-ppt/)  
- [OpenAI API](https://platform.openai.com/)  
- [Anthropic API](https://docs.anthropic.com/)  
- [Google Gemini](https://ai.google.dev/)  
