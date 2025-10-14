# ATS Resume Expert 🎯

An intelligent resume analysis tool powered by Google's Gemini AI that helps job seekers optimize their resumes for Applicant Tracking Systems (ATS). This application analyzes your resume against job descriptions and provides actionable insights to improve your chances of getting noticed by recruiters.

## 🌟 Demo

[Live Demo](https://ats-resume-expert-7g3gv28pip4t7gylrzurlk.streamlit.app/)

## ✨ Features

- **Resume Analysis**: Get professional evaluation of your resume against job descriptions
- **Skill Improvement Suggestions**: Receive personalized recommendations to enhance your skills
- **ATS Match Percentage**: Calculate how well your resume matches the job requirements
- **Keyword Analysis**: Identify missing keywords that ATS systems look for
- **AI-Powered Insights**: Leverage Google's Gemini 1.5 Flash model for intelligent analysis
- **PDF Support**: Upload resumes in PDF format for analysis

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or higher
- Google API Key (for Gemini AI)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Om-ingle/ATS-Resume-Expert.git
   cd ATS-Resume-Expert
   ```

2. **Create a virtual environment** (recommended)
   ```bash
   python -m venv venv
   
   # On Windows
   venv\Scripts\activate
   
   # On macOS/Linux
   source venv/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**
   
   Create a `.env` file in the root directory and add your Google API key:
   ```env
   GOOGLE_API_KEY=your_google_api_key_here
   ```
   
   To get a Google API key:
   - Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
   - Create a new API key
   - Copy and paste it into your `.env` file

### Running the Application

Start the Streamlit application:
```bash
streamlit run app.py
```

The application will open in your default web browser at `http://localhost:8501`

## 📖 Usage

1. **Enter Job Description**: Paste the job description in the text area
2. **Upload Resume**: Upload your resume in PDF format
3. **Choose Analysis Type**:
   - **Tell me About the Resume**: Get a professional evaluation of your resume
   - **How can I Improvise my skills**: Receive skill improvement suggestions
   - **Percentage match**: Get an ATS compatibility score with missing keywords

## 🛠️ Technology Stack

- **Frontend**: Streamlit
- **AI Model**: Google Gemini 1.5 Flash
- **PDF Processing**: PyMuPDF (fitz)
- **Image Processing**: Pillow (PIL)
- **Environment Management**: python-dotenv

## 📁 Project Structure

```
ATS-Resume-Expert/
├── app.py                  # Main Streamlit application
├── p.py                    # Utility script for listing Gemini models
├── requirements.txt        # Python dependencies
├── .env                    # Environment variables (create this)
├── .gitignore             # Git ignore rules
└── README.md              # Project documentation
```

## 🔧 Configuration

### For Streamlit Cloud Deployment

If deploying to Streamlit Cloud:

1. Go to your app settings in Streamlit Cloud
2. Navigate to "Secrets" section
3. Add your Google API key:
   ```toml
   GOOGLE_API_KEY = "your_google_api_key_here"
   ```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Create a Pull Request

## 📝 How It Works

1. **PDF Processing**: The application converts your resume PDF into an image format that the AI can analyze
2. **AI Analysis**: Google's Gemini AI processes the resume image along with the job description
3. **Intelligent Evaluation**: Based on the selected option, the AI provides:
   - Professional resume evaluation
   - Skill gap analysis and improvement suggestions
   - ATS compatibility score with keyword analysis

## ⚠️ Important Notes

- Ensure your Google API key has access to the Gemini API
- The application processes only the first page of multi-page resumes
- Internet connection is required for AI analysis
- Keep your API key secure and never commit it to version control

## 🐛 Troubleshooting

**Error: "Google API key not found"**
- Make sure you've created the `.env` file with your API key
- Verify the API key is correctly formatted

**Error: "Error generating response"**
- Check your internet connection
- Verify your API key is valid and active
- Ensure your Google Cloud project has the Gemini API enabled

**PDF Upload Issues**
- Make sure your resume is in PDF format
- Try reducing the file size if it's too large

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Author

**Om Ingle**

- GitHub: [@Om-ingle](https://github.com/Om-ingle)

## 🙏 Acknowledgments

- Google Generative AI team for the Gemini API
- Streamlit team for the amazing framework
- All contributors and users of this project

## 📞 Support

If you encounter any issues or have questions, please:
- Open an issue on GitHub
- Check existing issues for solutions
- Contact the maintainer

---

Made with ❤️ to help job seekers succeed in their career journey
