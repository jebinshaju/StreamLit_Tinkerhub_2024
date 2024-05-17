
![Streamlit notion](https://github.com/TH-Activities/saturday-hack-night-template/assets/117498997/e8052bb6-ad89-48c3-b6e9-124f94c1cd01)

# MyAnswer 🎤

MyAnswer is an innovative web application designed to enhance the viva voce experience for partially blind individuals. Leveraging the power of Vertex AI and generative AI, this app provides a seamless and effective platform for remote examinations and assessments. Teachers can create and manage tests, while students can participate in exams and receive instant feedback through audio and text.

## Team Members
1. [Name 1](https://github.com/TH-Activities/saturday-hack-night-template)
2. [Name 2](https://github.com/TH-Activities/saturday-hack-night-template)

## Link to Product Walkthrough
[Link to video](Link Here)

## How It Works
1. **Teacher Functionality**:
    - Teachers can sign up, log in, create tests, and manage questions.
    - Teachers can view student submissions and check their marks.
    - The app uses generative AI to evaluate student answers and provide detailed feedback.
2. **Student Functionality**:
    - Students can sign up, log in, and enter examination codes to start exams.
    - The app uses speech-to-text to capture student answers and provides audio feedback.
    - Students can view their previous exam results and receive instant feedback.

## Libraries Used
- Streamlit
- Pyrebase
- Vertex AI
- gTTS
- TemporaryFile
- Base64
- Re
- UUID
- json

## How to Configure
1. Clone the repository to your local machine.
   ```bash
   git clone https://github.com/your-repo/myanswer.git
   cd myanswer
   ```
2. Install the required libraries.
   ```bash
   pip install -r requirements.txt
   ```
3. Set up your Firebase project and configure the `firebaseConfig` in the app code.
4. Initialize Vertex AI with your project details.

## How to Run
1. Run the Streamlit app.
   ```bash
   streamlit run app.py
   ```
2. Access the app in your browser at `http://localhost:8501`.

## Deployment
This application is hosted on Google Cloud using Cloud Run. Follow the steps below to deploy:

1. **Build the Docker Image**:
   ```bash
   docker build -t myanswer .
   ```
2. **Push the Docker Image to Google Container Registry**:
   ```bash
   docker tag myanswer gcr.io/your-project-id/myanswer
   docker push gcr.io/your-project-id/myanswer
   ```
3. **Deploy to Cloud Run**:
   ```bash
   gcloud run deploy myanswer --image gcr.io/your-project-id/myanswer --platform managed
   ```

## Key Features
- **Accessibility**: Enhances the viva experience for partially blind students with audio-based interactions.
- **Generative AI**: Utilizes Vertex AI for evaluating student answers and generating detailed, explanatory feedback.
- **Instant Feedback**: Provides immediate feedback and results to students, making the learning process more efficient.
- **User-Friendly**: Simple and intuitive interface for both teachers and students, ensuring a seamless user experience.

## Conclusion
MyAnswer revolutionizes the viva voce process for partially blind individuals by integrating advanced AI technologies to create an inclusive, effective, and user-friendly examination platform. Join us in making education more accessible and engaging for everyone.

---

This project is part of a competition for Streamlit apps, showcasing innovative uses of generative AI and accessibility features.
