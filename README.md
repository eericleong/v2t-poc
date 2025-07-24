# V2T POC – Voice-to-Text Transcription Prototype

This is a proof-of-concept (POC) web interface that allows users to upload interview recordings, select a transcription language, and receive a transcribed output. The solution uses Cloudinary for video uploads and Make.com (formerly Integromat) for orchestration and webhook integration.

---

## 🧩 Features

- 🎥 Upload MP4 videos via the Cloudinary Upload Widget
- 🌍 Choose from multiple transcription languages (English, Spanish, French, German)
- 📡 Submit recordings through a Make.com webhook for processing
- 🔁 Poll automatically until transcription results are ready
- 🎬 Preview the uploaded video before submission
- ✨ Automatically summarize the meeting transcript using ChatGPT
- 🧾 View transcribed text in a syntax-highlighted code block
- 🖼 Generate a presentation slide based on summarized insights
- 📧 Create and send a polished HTML email with highlights and outcomes

---

## 🔧 How It Works

1. User selects a video file to upload via Cloudinary’s widget
2. The uploaded video URL is submitted to a Make.com webhook along with:
   - A selected language
   - A unique UUID for tracking
3. A second webhook is polled in intervals until transcription is complete
4. Once available, the transcript is shown in a preformatted viewer with syntax highlighting
5. Output files such as transcript, summary and slide are available in your Google Drive
6. A formatted email will appear in your inbox

---

## 📁 Files

- `v2t-poc.html` – Main frontend interface
- No backend required (Make.com handles processing)

---

## 🌐 Deployment

This site can be deployed using **GitHub Pages**:

1. Push your code to a public GitHub repo
2. Go to `Settings → Pages`
3. Choose the `main` branch and `/ (root)` directory
4. Visit: `https://your-username.github.io/v2t-poc/`

---

## 🚀 Stack

- HTML + JavaScript
- Cloudinary Upload Widget
- [highlight.js](https://highlightjs.org/) for syntax formatting
- Make.com (webhooks, logic)
- ChatGPT
- AssemblyAI
- Google Translate
- Google Docs

---

## 📌 Requirements

- Cloudinary(https://cloudinary.com/) account with:
  - A valid cloud name
  - An unsigned upload preset (with `resource_type: video`)
- Make.com account with:
  - One webhook to accept file URL & language
  - One webhook to serve polling responses
- OpenAI account
- AssemblyAI account
- Google Drive account


---

## 📸 Screenshots

<img width="1250" height="798" alt="image" src="https://github.com/user-attachments/assets/4b03c34a-d215-49c4-ba21-5baa941b29c8" />


---

## 🛡 License

This is a proof-of-concept for internal or prototype use. No license applied.

---

## 🙋‍♂️ Questions?

Feel free to open an issue or message the author.
