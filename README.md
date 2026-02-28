<p align="center">
  <img src="./img.png" alt="Project Banner" width="100%">
</p>

# [MEDIBOT] 🎯

## Basic Details

### Team Name: [SHEHACKS]

### Team Members
- Member 1: [ANN GEORGE] - [MACE]
- Member 2: [APARNA SAJEEV] - [MACE]

### Hosted Project Link
[https://github.com/anngeo123/Medical-chatbot/commit/9f5c6068c2c4eaf8ee3e7f35cf6593bf0ced43ae]

### Project Description
[MediBot is an interactive web application that leverages AI and location services to help users:

Enter their symptoms, age, sex, and location.

Receive possible medical conditions and recommended specialists via GPT-4 AI, presented in a concise, professional, and informational manner.

Find nearby doctors or hospitals in their city using Google Maps API, making healthcare more accessible.

The app is built using Streamlit, providing a clean, responsive, and user-friendly interface, accessible from any web browser.]

### The Problem statement
[Millions of people experience mild to moderate symptoms daily, but often struggle to determine the possible causes or which specialist to consult. Accessing nearby doctors or hospitals can also be time-consuming, especially in unfamiliar areas. Existing solutions are either limited to textual databases or rely on complex manual search, leaving users uncertain and anxious about their health.

There is a clear need for a quick, interactive, and reliable tool that guides users in understanding their symptoms and locating nearby medical care without replacing professional consultation.]

### The Solution
[MediBot solves the problem by combining AI-powered symptom analysis with geolocation-based doctor search:

Symptom Analysis: GPT-4 processes user inputs to generate informational medical advice with recommended specialists.

Doctor Finder: Google Maps API identifies nearby hospitals and doctors for prompt access to healthcare.

User-Friendly Interface: Streamlit ensures users can interact intuitively, without technical knowledge.

This solution provides a fast, reliable, and safe first step for users to understand their symptoms and find medical help — all in one place.]

---

## Technical Details

### Technologies/Components Used

**For Software:**
- Languages used: [ Python]
- Frameworks used: [streamlit]
- Libraries used:openai,requests
- Tools used:[VS Code, Git, Google Cloud Console (for API keys) ]

**For Hardware:**
- Main components: [List main components]
- Specifications: [Technical specifications]
- Tools required: [List tools needed]

---

## Features

List the key features of your project:
- Feature 1: AI-Powered Symptom Analysis – Users enter their symptoms, age, sex, and location, and GPT-4 provides a list of possible conditions and recommended specialists in a concise, professional manner.
- Feature 2: Nearby Doctor & Hospital Finder – The app uses Google Maps API to locate nearby doctors or hospitals based on the user’s location.
- Feature 3: User-Friendly Interface – Built with Streamlit, the web app is interactive, responsive, and easy to use, requiring no technical knowledge.
- Feature 4: Informational & Safe – All advice is purely informational with a clear disclaimer, guiding users without replacing professional medical consultation.

---

## Implementation

### For Software:

#### Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/medibot.git
cd medibot

# Install required Python libraries
pip install -r requirements.txt



#### Run
```bash<img width="461" height="1181" alt="medibot" src="https://github.com/user-attachments/assets/6b7453c0-57eb-4c56-838d-938cf20888fe" />

# Run the Streamlit app
streamlit run medibot_web_gpt_google.py

### For Hardware:

#### Components Required
[List all components needed with specifications]

#### Circuit Setup
[Explain how to set up the circuit]

---

## Project Documentation

### For Software:

#### Screenshots (Add at least 3)

![Screenshot1](Add screenshot 1 here with proper name)
*Add caption explaining what this shows*

![Screenshot2](Add screenshot 2 here with proper name)
*Add caption explaining what this shows*

![Screenshot3](Add screenshot 3 here with proper name)
*Add caption explaining what this shows*

#### Diagrams

**System Architecture:**

![Architecture Diagram](docs/architecture.png)
*Explain your system architecture - components, data flow, tech stack interaction*

**Application Workflow:**
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/3f689317-8d13-4579-8538-146f78fec63b" />

<img width="461" height="1181" alt="medibot" src="https://github.com/user-attachments/assets/d39bd6d2-5891-41b2-b5c3-8c226420ff94" />

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/b8564088-cb6b-4707-a513-83de2fe93970" />

![Workflow](docs/workflow.png)
This diagram illustrates the MediBot application workflow. The user enters their symptoms, age, sex, and location through the Streamlit interface. The input is sent to GPT-4, which generates possible medical conditions and recommends appropriate specialists. Simultaneously, the location is sent to the Google Maps API to find nearby doctors and hospitals. Finally, all results are displayed back to the user along with an informational disclaimer, completing the end-to-end workflow.

---

### For Hardware:

#### Schematic & Circuit

![Circuit](Add your circuit diagram here)
*Add caption explaining connections*

![Schematic](Add your schematic diagram here)
*Add caption explaining the schematic*

#### Build Photos

![Team](Add photo of your team here)

![Components](Add photo of your components here)
*List out all components shown*

![Build](Add photos of build process here)
*Explain the build steps*

![Final](Add photo of final product here)
*Explain the final build*

---

## Additional Documentation

### For Web Projects with Backend:

#### API Documentation
OPENAI GPT API:
**Base URL:** `https://api.openai.com`
Google Maps Places API: https://maps.googleapis.com/maps/api/place/textsearch/json

##### Endpoints

**GET /api/endpoint**
- **Description:** Generates possible medical conditions and recommends specialists based on user symptoms.
- **Parameters:**
  - `query` (string): Search query, e.g., "doctors in Kochi"
  - `key` (string): google maps api key
- **Response:**
{
  "results": [
    {
      "name": "City Hospital",
      "formatted_address": "123 Main St, Kochi",
      "geometry": { "location": {"lat": 10.0, "lng": 76.0} }
    }
  ]}

**POST /api/endpoint**
- **Description:** Generates possible medical conditions and recommends specialists based on user symptoms.
- **Request Body:**
{
  "model": "gpt-4.1-mini",
  "messages": [
    {
      "role": "user",
      "content": "I have fever and headache, age 25, male, in Kochi"
    }
  ],
  "temperature": 0.5
}
```
- **Response:**
```json
{
  "choices": [
    {
      "message": {
        "content": "Possible Conditions: 1. Viral Fever, 2. Migraine. Recommended Specialists: General Physician, Neurologist."
      }
    }
  ]
}
```

[Add more endpoints as needed...]

---

### For Mobile Apps:

#### App Flow Diagram

![App Flow](<img width="461" height="1181" alt="medibot" src="https://github.com/user-attachments/assets/ca254c8f-ed9f-44ab-9dfc-2f31e1755e0a" />
)
*Explain the user flow through your application*
This diagram shows the end-to-end workflow of MediBot. The user enters symptoms, age, sex, and location through the Streamlit interface. The input is sent to the GPT-4 API, which generates possible medical conditions and recommends specialists. Simultaneously, the location is sent to the Google Maps API to retrieve nearby doctors and hospitals. Finally, all results are displayed back to the user in a clear, user-friendly interface along with an informational disclaimer.


#### Installation Guide

**For Android (APK):**
1. Download the APK from [Release Link]
2. Enable "Install from Unknown Sources" in your device settings:
   - Go to Settings > Security
   - Enable "Unknown Sources"
3. Open the downloaded APK file
4. Follow the installation prompts
5. Open the app and enjoy!

**For iOS (IPA) - TestFlight:**
1. Download TestFlight from the App Store
2. Open this TestFlight link: [Your TestFlight Link]
3. Click "Install" or "Accept"
4. Wait for the app to install
5. Open the app from your home screen

**Building from Source:**
```bash
# For Android
flutter build apk
# or
./gradlew assembleDebug

# For iOS
flutter build ios
# or
xcodebuild -workspace App.xcworkspace -scheme App -configuration Debug
```

---

### For Hardware Projects:

#### Bill of Materials (BOM)

| Component | Quantity | Specifications | Price | Link/Source |
|-----------|----------|----------------|-------|-------------|
| Arduino Uno | 1 | ATmega328P, 16MHz | ₹450 | [Link] |
| LED | 5 | Red, 5mm, 20mA | ₹5 each | [Link] |
| Resistor | 5 | 220Ω, 1/4W | ₹1 each | [Link] |
| Breadboard | 1 | 830 points | ₹100 | [Link] |
| Jumper Wires | 20 | Male-to-Male | ₹50 | [Link] |
| [Add more...] | | | | |

**Total Estimated Cost:** ₹[Amount]

#### Assembly Instructions

**Step 1: Prepare Components**
1. Gather all components listed in the BOM
2. Check component specifications
3. Prepare your workspace
![Step 1](images/assembly-step1.jpg)
*Caption: All components laid out*

**Step 2: Build the Power Supply**
1. Connect the power rails on the breadboard
2. Connect Arduino 5V to breadboard positive rail
3. Connect Arduino GND to breadboard negative rail
![Step 2](images/assembly-step2.jpg)
*Caption: Power connections completed*

**Step 3: Add Components**
1. Place LEDs on breadboard
2. Connect resistors in series with LEDs
3. Connect LED cathodes to GND
4. Connect LED anodes to Arduino digital pins (2-6)
![Step 3](images/assembly-step3.jpg)
*Caption: LED circuit assembled*

**Step 4: [Continue for all steps...]**

**Final Assembly:**
![Final Build](images/final-build.jpg)
*Caption: Completed project ready for testing*

---

### For Scripts/CLI Tools:

#### Command Reference

**Basic Usage:**
```bash
python medibot.py [options]
```

**Available Commands:**
--city CITY – Specify city for doctor search

--symptoms "text" – Provide symptoms directly (non-interactive mode)

--age AGE – Specify patient age

--sex SEX – Specify patient sex (male/female/other)

--format json – Return output in JSON format

--nearby – Fetch nearby doctors

--no-ai – Skip AI diagnosis (only show nearby doctors)
**Options:**
-h, --help – Show help message and exit

-v, --verbose – Enable detailed processing logs

-o, --output FILE – Save results to a file

--version – Show MediBot version
**Examples:**

```bash
python medibot.py


```

#### Demo Output

**Example 1: Basic Processing**

**Input:**
Welcome to MediBot!
Enter your city: Kochi
Enter your age: 20
Enter your sex: Female
Enter your symptoms: fever and headache

Analyzing symptoms...
Possible Conditions:
- Viral Fever
- Flu

Recommended Specialist:
- General Physician

Searching nearby doctors in Kochi...

Nearby Doctors:
1. Dr. -- Clinic
2. -- Hospital

Disclaimer: This is not a medical diagnosis.
**Command:**
```bash
python medibot.py --city Kochi --age 20 --sex female --symptoms "fever and headache"
```

**Output:**

Processing request...
Possible Conditions:
- Viral Fever
- Flu

Recommended Specialist:
- General Physician

Nearby Doctors in Kochi:
- ABC Hospital
- Sunrise Medical Center
**Example 2: Advanced Usage**

**Input:**
```json
{
  "name": "test",
  "value": 123
}
```

**Command:**
```bash
python medibot.py -v --city Kochi --symptoms "stomach pain"
```

**Output:**
```
[VERBOSE] Loading API keys...
[VERBOSE] Sending request to GPT API...
[VERBOSE] Fetching nearby doctors via Maps API...
[VERBOSE] Processing results...

Possible Conditions:
- Gastritis
- Food Poisoning

Specialist:
- Gastroenterologist
--
## Project Demo

### Video
[Add your demo video link here - YouTube, Google Drive, etc.]

*Explain what the video demonstrates - key features, user flow, technical highlights*

### Additional Demos
[Add any extra demo materials/links - Live site, APK download, online demo, etc.]

---

## AI Tools Used (Optional - For Transparency Bonus)

If you used AI tools during development, document them here for transparency:

**Tool Used:**  GitHub Copilot,ChatGPT, Google ai studio

**Purpose:** [What you used it for]
-Generated initial boilerplate code for Streamlit frontend
-Assisted in GPT API integration and configuration
-Debugging Python errors and virtual environment issues
-Suggesting improvements for API structure and CLI arguments
-Helping design system architecture and workflow diagram
-Formatting documentation and README sections

**Key Prompts Used:**
"Create a medical chatbot using Python and GPT API"

"Integrate Google Maps API to fetch nearby doctors"

"Fix ModuleNotFoundError in virtual environment"

**Percentage of AI-generated code:** [Approximately 60%]

**Human Contributions:**
- Architecture design and planning
- Custom business logic implementation
- Integration and testing
- UI/UX design decisions

*Note: Proper documentation of AI usage demonstrates transparency and earns bonus points in evaluation!*

---

## Team Contributions

- [ann]: .Frontend development using Streamlit]
- [aparna]: Testing and debugging

Documentation and README preparation

---

## License

This project is licensed under the [LICENSE_NAME] License - see the [LICENSE](LICENSE) file for details.

**Common License Options:**
- MIT License (Permissive, widely used)
- Apache 2.0 (Permissive with patent grant)
- GPL v3 (Copyleft, requires derivative works to be open source)

---

Made with ❤️ at TinkerHub
