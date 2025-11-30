# 🤖 AI-Powered Resume Critic

A comprehensive web application that analyzes resumes using advanced NLP techniques and provides actionable insights to improve ATS compatibility and overall resume quality.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Streamlit](https://img.shields.io/badge/Streamlit-1.28+-red.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://ai-powered-resume-critic.streamlit.app/)

## 🚀 Live Demo

**👉 [Try it Now - AI Resume Critic](https://ai-powered-resume-critic.streamlit.app/)**

Upload your resume and get instant, comprehensive analysis with actionable recommendations!

---

## 📊 Overview

AI-Powered Resume Critic uses machine learning and natural language processing to evaluate your resume across multiple dimensions, helping you optimize it for Applicant Tracking Systems (ATS) and recruiters.

### Why Use This Tool?

- **Beat ATS Systems**: 75% of resumes never reach human eyes. Ensure yours does.
- **Data-Driven Insights**: Get objective scores based on industry standards
- **Instant Feedback**: No waiting - analyze your resume in seconds
- **Free & Private**: No registration required, no data stored

---

## 🌟 Key Features

### 📈 Advanced Scoring System
- **ATS Compatibility Score** (100-point scale)
  - Text quality analysis (20 points)
  - Section completeness (40 points)
  - Formatting assessment (20 points)
  - Readability metrics (20 points)

### 🔍 Intelligent Analysis
- **Section Detection**: Automatically identifies 8 critical resume sections
  - Contact Information
  - Professional Summary
  - Work Experience
  - Education
  - Skills
  - Projects
  - Certifications
  - Awards

### 🎯 Keyword Optimization
- **5 Category Analysis** with weighted scoring:
  - **Technical Skills** (1.5x weight): Python, AWS, Docker, ML, etc.
  - **Certifications** (1.4x weight): PMP, AWS Certified, Six Sigma, etc.
  - **Business Terms** (1.3x weight): ROI, KPI, Strategy, Revenue, etc.
  - **Action Verbs** (1.2x weight): Managed, Implemented, Led, etc.
  - **Soft Skills** (1.0x weight): Leadership, Communication, etc.

### 📊 Visual Analytics
- **Interactive Dashboards**
  - Real-time gauge charts
  - Keyword frequency analysis
  - Section completeness visualization
  - Industry benchmark comparison

### 💡 Smart Recommendations
- **Personalized Suggestions**: Context-aware tips based on your gaps
- **Priority Action Items**: Ranked by impact potential
- **Level-Specific Advice**: Tailored for Entry/Mid/Senior roles

### 📉 Quantifiable Metrics
- Extracts impact data: percentages, dollar amounts, team sizes
- Identifies achievement-oriented language
- Highlights measurable results

---

## 🛠️ Technology Stack

- **Frontend**: Streamlit 1.28+
- **PDF Processing**: PyMuPDF (fitz)
- **Data Analysis**: Pandas, NumPy
- **Visualizations**: Plotly
- **NLP**: Scikit-learn, TextStat
- **Deployment**: Streamlit Cloud

---

## 💻 Local Installation

### Prerequisites
- Python 3.8 or higher
- pip package manager

### Setup

```bash
# Clone the repository
git clone https://github.com/Hat-GitBot/AI-Powered-Resume-Critic.git
cd AI-Powered-Resume-Critic

# Install dependencies
pip install -r requirements.txt

# Run the application
streamlit run app.py
```

The app will open in your browser at `http://localhost:8501`

### Requirements
```txt
streamlit>=1.28.0
PyMuPDF>=1.23.0
numpy>=1.24.0
plotly>=5.17.0
scikit-learn>=1.3.0
pandas>=2.0.0
textstat>=0.7.3
```

---

## 📖 How It Works

### 1. **PDF Text Extraction**
Uses PyMuPDF to extract text from uploaded resumes with page-by-page analysis.

### 2. **Multi-Factor ATS Scoring**
```
ATS Score = Text Quality (20%) + 
            Section Completeness (40%) + 
            Formatting (20%) + 
            Readability (20%)
```

### 3. **Weighted Keyword Analysis**
Keywords are categorized and weighted by importance to provide a comprehensive keyword strength score.

### 4. **Section Detection**
Pattern matching algorithms identify essential resume sections and flag missing components.

### 5. **Experience Level Assessment**
Analyzes years of experience and job titles to determine career stage automatically.

---

## 📊 Scoring Guide

### ATS Score Interpretation

| Score Range | Rating | Description |
|-------------|--------|-------------|
| 85-100 | 🌟 Excellent | Fully ATS-optimized, ready to submit |
| 70-84 | ✅ Good | Minor improvements recommended |
| 50-69 | ⚠️ Fair | Multiple areas need attention |
| 0-49 | ❌ Poor | Significant improvements required |

### Keyword Score

| Score Range | Strength | Action Needed |
|-------------|----------|---------------|
| 60-100 | Strong | Well-optimized with relevant keywords |
| 30-59 | Moderate | Add more industry-specific terms |
| 0-29 | Limited | Significant keyword enhancement needed |

---

## 🎯 Use Cases

### For Job Seekers
- Optimize resume for ATS systems before applying
- Identify missing sections and keywords
- Improve readability and formatting
- Track improvements over time

### For Career Coaches
- Provide data-driven feedback to clients
- Demonstrate resume improvements objectively
- Save time on initial assessment
- Focus on high-impact changes

### For Recruiters
- Quick resume quality assessment
- Screen candidates efficiently
- Maintain consistent evaluation standards

### For Students
- Learn resume best practices
- Understand industry standards
- Build ATS-friendly resumes from scratch

---

## ⚠️ Limitations

- **Text-Based PDFs Only**: Requires machine-readable text (not scanned images)
- **File Size Limit**: Maximum 10MB per upload
- **Language**: Currently optimized for English resumes
- **General ATS Scoring**: Based on best practices, not specific ATS platforms

---

## 🔐 Privacy & Security

- **No Data Storage**: All resumes are processed in-memory only
- **No Registration**: Use the tool without creating an account
- **Temporary Processing**: Data is cleared immediately after analysis
- **Secure**: All processing happens server-side with HTTPS encryption

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

### Ways to Contribute
1. **Report Bugs**: [Open an issue](https://github.com/Hat-GitBot/AI-Powered-Resume-Critic/issues)
2. **Suggest Features**: Share your ideas for improvements
3. **Submit Pull Requests**: Fix bugs or add features
4. **Improve Documentation**: Help make the docs clearer
5. **Share Feedback**: Let us know how we can improve

### Development Setup

```bash
# Fork the repository
# Clone your fork
git clone https://github.com/Hat-GitBot/AI-Powered-Resume-Critic.git

# Create a feature branch
git checkout -b feature/amazing-feature

# Make your changes and commit
git commit -m 'Add some amazing feature'

# Push to your fork
git push origin feature/amazing-feature

# Open a Pull Request
```

---

## 🙏 Acknowledgments

- **[Streamlit](https://streamlit.io/)** - For the amazing web framework
- **[PyMuPDF](https://pymupdf.readthedocs.io/)** - For reliable PDF processing
- **[Plotly](https://plotly.com/)** - For interactive visualizations
- **[TextStat](https://github.com/shivam5992/textstat)** - For readability metrics
- **Open Source Community** - For inspiration and support

---

## 📧 Contact & Support

### Get Help
- **Issues**: [GitHub Issues](https://github.com/Hat-GitBot/AI-Powered-Resume-Critic/issues)
- **Discussions**: [GitHub Discussions](https://github.com/Hat-GitBot/AI-Powered-Resume-Critic/discussions)

### Share Your Experience
- ⭐ **Star this repo** if you found it helpful
- 🐦 **Tweet about it** and tag us
- 📝 **Write a blog post** about your experience
- 💬 **Share with friends** who are job hunting

### Connect
- **GitHub**: [Hat-GitBot](https://github.com/Hat-GitBot)
-  **LinkedIn**:  [Deepak Shamsheer](https://www.linkedin.com/in/deepak-shamsheer-6099b8212)
-  **Email**:  [gitbotdown@gmail.com](mailto:gitbotdown@gmail.com)
- **Live App**: [Try it Now](https://ai-powered-resume-critic.streamlit.app/)

---

<div align="center">

## 💼 Built for Job Seekers, By Job Seekers

**Made with ❤️ to help everyone land their dream job**

[🌐 Live Demo](https://ai-powered-resume-critic.streamlit.app/) •  [📂 GitHub](https://github.com/Hat-GitBot/AI-Powered-Resume-Critic) •  [🐛 Report Bug](https://github.com/Hat-GitBot/AI-Powered-Resume-Critic/issues) • [✨ Request Feature](https://github.com/Hat-GitBot/AI-Powered-Resume-Critic/issues)

---

⭐ **Star this repo if it helped you land an interview!**

---

*Last Updated: November 2025*

</div>
