# ATS Resume Application Tracking System

This project is a comprehensive **Application Tracking System (ATS)** built using **Google Generative AI** and **Streamlit**. The ATS helps job applicants improve their resumes by matching them with job descriptions, calculating a percentage match, and suggesting areas for improvement. This tool is ideal for understanding how resumes align with specific roles and optimizing job applications for modern hiring systems.

---

## **Features**

- **Resume Upload**: Upload your resume in PDF format for analysis.
- **Job Description Input**: Enter the job description text to match it against your resume.
- **Percentage Match Calculation**: View how well your resume matches the job description.
- **Keyword Suggestions**: Identify missing keywords and areas for improvement.
- **Insights from Google Generative AI**: Leverage advanced AI models to analyze and generate professional suggestions.
- **User-Friendly Interface**: Built with Streamlit for a smooth and interactive experience.

---

## **Tech Stack**

- **Frontend**: Streamlit
- **AI Integration**: Google Generative AI (Gemini models)
- **Backend**: Python
- **Libraries Used**:
  - `streamlit` (for building the web application)
  - `google-generativeai` (for AI-powered insights)
  - `pdf2image` (for converting PDF resumes to images)
  - `Pillow` (for image processing)
  - `base64` (for encoding images)
  - `dotenv` (for managing API keys securely)

---

## **Setup and Installation**

Follow these steps to set up and run the project:

1. **Clone the Repository**:
   ```bash
   git clone <repository_url>
   cd <repository_directory>
   ```

2. **Create a Virtual Environment**:
   ```bash
   python -m venv env
   source env/bin/activate  # For Linux/Mac
   .\env\Scripts\activate  # For Windows
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up API Key**:
   - Obtain your API key from Google Cloud Console.
   - Create a `.env` file in the project root directory and add your API key:
     ```env
     GOOGLE_API_KEY=your_google_api_key
     ```

5. **Run the Application**:
   ```bash
   streamlit run app.py
   ```

---

## **How It Works**

1. **Upload Resume**:
   - Users can upload their resumes in PDF format using the upload button.

2. **Enter Job Description**:
   - Users input the job description in a text box.

3. **Analysis**:
   - The system processes the uploaded resume using `pdf2image` to extract key information.
   - The AI model evaluates the resume against the job description.

4. **Output**:
   - **Percentage Match**: The similarity score between the resume and job description.
   - **Keyword Suggestions**: Identifies missing keywords to optimize the resume.
   - **Professional Feedback**: Suggestions on how to align the resume with the job requirements.

---

## **Prompts Used**

### Prompt 1: Resume Evaluation
```plaintext
You are an experienced HR with technical expertise in roles such as Data Science, Full Stack Development, or DevOps. Review the provided resume against the job description and share professional feedback. Highlight strengths and weaknesses in alignment with the job requirements.
```

### Prompt 2: ATS Keyword Analysis
```plaintext
You are an ATS expert with a deep understanding of resume parsing and keyword matching. Analyze the provided resume against the job description and output the following:
1. Percentage match.
2. Missing keywords.
3. Final recommendations for improvement.
```

---

## **Sample Outputs**


![WhatsApp Image 2025-01-12 at 00 37 58_e5cee226](https://github.com/user-attachments/assets/2df24d86-37f4-4794-b462-110c6f8e7f7a)
![WhatsApp Image 2025-01-12 at 00 38 16_15165f7d](https://github.com/user-attachments/assets/f18a3937-72bb-4add-8901-38a5b7fbf6ae)
![WhatsApp Image 2025-01-12 at 00 38 57_2dde7bb2](https://github.com/user-attachments/assets/6ae00efb-bd2b-494b-99e6-3aa13d5bf50f)
![WhatsApp Image 2025-01-12 at 00 39 19_fc9e552a](https://github.com/user-attachments/assets/324b3a68-0433-4dad-ac8c-43ab412f18ea)





