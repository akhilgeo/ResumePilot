# ResumePilot 🚀

**AI-Powered Resume Builder with Multiple ATS-Ready Templates**

ResumePilot is a comprehensive, AI-enhanced resume builder that helps you create professional, ATS-optimized resumes in minutes. Built with modern web technologies and powered by AI, it offers intelligent suggestions to make your resume stand out.



---

## ✨ Features

### 🤖 AI-Powered Assistance
- **Auto-Generate Professional Summary**: AI analyzes your experience and skills to create compelling summaries
- **Enhance Job Descriptions**: Transform basic descriptions into impactful, achievement-focused statements
- **Smart Skill Suggestions**: Get relevant skill recommendations based on your job titles and experience

### 📄 Multiple ATS-Ready Templates
- **Classic Professional**: Traditional format perfect for corporate roles
- **Modern Minimal**: Clean, contemporary design with gradient accents
- **Two-Column Layout**: Efficient space utilization for comprehensive resumes

### 💼 Comprehensive Resume Sections
- Personal Information with profile picture support
- Professional Summary
- Work Experience (unlimited entries)
- Education History
- Skills with tag-based interface
- Real-time preview as you type

### 📥 Export Options
- **PDF Download**: High-quality PDF generation
- **DOCX Download**: Editable Microsoft Word format
- Both formats preserve formatting and are ATS-compatible

---

## 🖼️ Screenshots

### Main Interface

*Split-screen interface with form editor on the left and live preview on the right*

### Personal Information Section

*Easy-to-fill personal details with profile picture upload*

### AI-Powered Summary Generation

*Click to generate professional summaries based on your experience*

### Work Experience with AI Enhancement

*Add multiple jobs and enhance descriptions with AI*

### Template Selection

*Three professional templates to choose from*

### Classic Template Preview

*Traditional, clean design perfect for any industry*

### Modern Template Preview

*Contemporary design with vibrant accents*

### Two-Column Template Preview

*Maximizes space with sidebar layout*

### Export Options

*One-click download in your preferred format*

---

## 🚀 Getting Started

### Option 1: Use Online (Recommended)
1. Open the `index.html` file in your web browser
2. Start filling in your information
3. Use AI features to enhance your content
4. Choose your template
5. Download your resume!

### Option 2: Run with Local Server
If you encounter CORS issues with AI features, use a local server:

**Using Python:**
```bash
python -m http.server 8000
```
Then open `http://localhost:8000` in your browser.

**Using Node.js:**
```bash
npx http-server
```

**Using VS Code:**
Install the "Live Server" extension and right-click on `index.html` → "Open with Live Server"

---

## 🛠️ Technical Stack

- **Frontend**: Pure HTML5, CSS3, JavaScript (ES6+)
- **AI Integration**: OpenRouter API with Llama 3.2 model
- **PDF Generation**: jsPDF + html2canvas
- **DOCX Generation**: docx.js library
- **CDN Libraries**: 
  - jsPDF 2.5.1
  - html2canvas 1.4.1
  - docx 7.8.2

---

## 🔑 API Configuration

ResumePilot uses OpenRouter API for AI features. The API key is already configured in the code, but you can replace it with your own:

```javascript
const OPENROUTER_API_KEY = 'your-api-key-here';
```

Get your free API key at [OpenRouter.ai](https://openrouter.ai/)

---

## 📋 How to Use

### Step 1: Personal Information
1. Upload a professional profile picture (optional)
2. Fill in your name, email, phone, location
3. Add LinkedIn profile URL

### Step 2: Work Experience
1. Click "Add Experience" to add jobs
2. Fill in job title, company, dates, and description
3. Click "🤖 Enhance with AI" to improve your descriptions
4. Add multiple positions as needed

### Step 3: Education
1. Click "Add Education" to add degrees
2. Enter degree, institution, graduation date, and GPA
3. Add multiple educational qualifications

### Step 4: Skills
1. Type a skill and press Enter to add
2. Or click "🤖 Suggest Skills" for AI recommendations
3. Remove skills by clicking the × on any skill tag

### Step 5: Professional Summary
1. Write your own summary, or
2. Click "🤖 Generate AI Summary" for automatic creation
3. Edit as needed

### Step 6: Choose Template
Select from three professional templates:
- **Classic**: Best for traditional industries
- **Modern**: Great for creative/tech roles
- **Two-Column**: Perfect for comprehensive resumes

### Step 7: Download
Click either:
- **📄 Download PDF**: For online applications
- **📝 Download DOCX**: For further editing

---

## 🎨 Customization

### Changing Colors
Edit the CSS variables in the `<style>` section:

```css
/* Primary gradient colors */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);

/* Section colors */
.section h2 {
    color: #667eea;
}
```

### Adding More Templates
1. Create a new template class in CSS (e.g., `.template-creative`)
2. Add a template option in the HTML
3. Update the `selectTemplate()` function

### Modifying AI Prompts
Edit the prompts in the AI functions to customize output style:

```javascript
const prompt = `Your custom instructions here...`;
```

---

## 🔒 Privacy & Security

- **No Data Storage**: All data stays in your browser's memory
- **No Server Communication**: Except for AI API calls
- **Secure API Calls**: Using HTTPS encryption
- **Local Processing**: Resume generation happens in your browser

**Note**: Be cautious when sharing the HTML file as it contains the API key.

---

## 🐛 Troubleshooting

### AI Features Not Working
- **Solution 1**: Use a local web server (not file://)
- **Solution 2**: Check browser console for error messages
- **Solution 3**: Verify API key is valid

### PDF Export Issues
- **Check**: Ensure all CDN libraries are loading
- **Try**: Refresh the page and try again
- **Alternative**: Use DOCX export instead

### Profile Picture Not Showing
- **Check**: File size (keep under 5MB)
- **Format**: Use JPG, PNG, or GIF
- **Try**: Different browser if issue persists

### Template Not Switching
- **Refresh**: Clear browser cache
- **Click**: Ensure you're clicking the template boxes
- **Check**: JavaScript console for errors

---

## 📱 Browser Compatibility

✅ Chrome 90+
✅ Firefox 88+
✅ Safari 14+
✅ Edge 90+
✅ Opera 76+

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Report Bugs**: Open an issue with details
2. **Suggest Features**: Share your ideas
3. **Improve Code**: Submit pull requests
4. **Add Templates**: Design new resume layouts
5. **Enhance AI**: Improve prompt engineering

---

## 📄 License

This project is open source and available under the MIT License.

```
MIT License

Copyright (c) 2026 ResumePilot

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 🌟 Acknowledgments

- **AI Models**: Powered by Meta's Llama 3.2 via OpenRouter
- **Icons**: Emoji-based for universal compatibility
- **Design Inspiration**: Modern resume best practices
- **Community**: Thanks to all contributors and users

---

## 📞 Support

Need help? Have questions?

- 📧 Email: support@resumepilot.ai
- 💬 Discord: [Join our community](#)
- 🐛 Issues: [GitHub Issues](#)
- 📚 Docs: [Full Documentation](#)

---

## 🗺️ Roadmap

### Coming Soon
- [ ] More template options
- [ ] Cover letter generator
- [ ] LinkedIn profile optimization
- [ ] Resume scoring and ATS checker
- [ ] Multi-language support
- [ ] Save/load resume functionality
- [ ] Custom color themes
- [ ] Mobile app version

---

## ⭐ Star Us!

If you find ResumePilot helpful, please consider giving it a star on GitHub! It helps others discover this tool.

---

<div align="center">

**Built with ❤️ for job seekers worldwide**

[Website](#) • [Demo](#) • [Documentation](#) • [Report Bug](#) • [Request Feature](#)

</div>

---

## 📊 Stats

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![AI Powered](https://img.shields.io/badge/AI-Powered-purple)
![ATS Ready](https://img.shields.io/badge/ATS-Ready-orange)

---

**Made with 💼 ResumePilot - Your AI Co-Pilot for Career Success**