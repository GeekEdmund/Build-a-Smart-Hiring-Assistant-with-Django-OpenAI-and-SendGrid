
# ML Engineer Application

This project is a web application designed for candidates to apply for a Machine Learning Engineer position. It allows users to upload their resumes, which are then processed and assessed against predefined job qualifications using advanced services like RAG, OpenAI's API and SendGrid for communication.
Feel free to customize it to meet your specific requirements.
## Features

- **Resume Upload**: Users can upload their resumes in PDF format.
- **Resume Assessment**: Resumes are evaluated against specific job qualifications using AI.
- **Automated Communication**: Candidates receive feedback via email regarding their application status.
- **User-Friendly Interface**: A responsive and visually appealing user interface built with Tailwind CSS.

## Technologies Used

- **Django**: The web framework that serves as the backbone of the application.
- **Python-dotenv**: For managing environment variables.
- **OpenAI**: To analyze resumes and extract qualifications.
- **SendGrid**: For sending automated emails to candidates.
- **PDFMiner**: To extract text from PDF resumes.
- **Python-magic**: For file type identification.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/ml-engineer-application.git
   ```

2. Install the required packages:

   ```bash
   pip install django python-dotenv openai sendgrid pdfminer.six python-magic
   ```

3. Set up your environment variables. Create a `.env` file in the root directory and add your OpenAI API key, SendGrid API key, and email configuration:

   ```plaintext
   OPENAI_API_KEY=your_openai_api_key
   SENDGRID_API_KEY=your_sendgrid_api_key
   MAIL_FROM_ADDRESS=your_email@example.com
   MAIL_FROM_NAME="Your Name"
   RECRUITER_EMAIL=your_recruiter_email@example.com
   ```

4. Run the migrations to set up the database:

   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

5. Start the development server:

   ```bash
   python manage.py runserver
   ```

6. Navigate to `http://127.0.0.1:8000/` in your web browser to access the application.

## Usage

1. Fill in your details and upload your resume in PDF format.
2. Submit the application.
3. Receive feedback via email regarding your application status.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue for any feature requests or bugs.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
