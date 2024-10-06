# AI Virtual Travel Agent

:warning: **This service is currently in production.**

AI-powered travel planning service that integrates real-time data from various sources to deliver optimized, personalized vacation itineraries. Our multi-agent architecture ensures every trip is tailored to the user's preferences, offering a seamless vacation planning experience.

## Key Features

- **Real-time Data Integration**: Leverages the **Tavily API** to pull live data from travel agencies, accommodations, and tourism platforms.
- **Multi-agent Architecture**: Combines AI agents for efficient query handling and itinerary generation, ensuring faster response times and user satisfaction.
- **Iterative Feedback Loop**: The Planner Critique Agent provides continuous feedback, refining the itinerary to meet the user's exact requirements.
- **Customization**: Supports personalized itineraries with a wide range of options, from adventure trips to family-friendly experiences.
- **User-Friendly Interface**: Designed to offer a seamless and intuitive experience, making vacation planning hassle-free.

## Technology Stack

- **Frontend**:
  - **Languages**: HTML, CSS, JavaScript
  - **Key Features**: Smooth scrolling, responsive design for desktop and mobile, cross-browser compatibility
- **Backend**:
  - **Languages/Frameworks**: Node.js, Express
  - **Key Features**: RESTful APIs, secure authentication, optimized routing, real-time data fetching
- **Database**:
  - **Type**: MySQL
  - **Purpose**: Stores user profiles, itinerary data, preferences, and past trips for personalized recommendations
- **API**: 
  - **Source**: Tavily API for live travel data (accommodations, activities, transportation)
  - **Function**: Real-time itinerary updates based on availability, user preferences, and current trends
- **AI Agents**:
  - **Language**: Python
  - **Libraries**: Pandas, Numpy, Scikit-learn for logic handling, data processing, and itinerary evaluation
- **Hosting**: 
  - **Planned Platforms**: AWS or Heroku for scalability, reliability, and performance

## Additional Features

- **Feedback Loop**: Continuous improvement through feedback from the Planner Critique Agent.
- **User Customization**: Personalized travel experiences, including adventure, family-friendly activities, and cultural experiences.
- **Mobile Responsiveness**: Optimized for a seamless experience across all devices.
- **Third-party Integrations**: Upcoming support for services like Booking.com and Google Maps.

## Installation and Setup

### Prerequisites

- **Python**: Ensure you have Python and `pip` installed. If not, you can download them from the [official Python website](https://www.python.org/downloads/).
- **Node.js**: Install Node.js and npm (Node package manager) from [Node.js official website](https://nodejs.org/).

### How to Run the Project

1. **Clone the repository:**
    ```bash
    git clone https://github.com/asif-mp3/AI-Virtual-Travel-Agent.git
    ```

2. **Navigate into the project directory:**
    ```bash
    cd AI-Virtual-Travel-Agent
    ```

3. **Install backend dependencies:**
    ```bash
    npm install
    ```

4. **Install Python dependencies:**
    - First, make sure you have Python set up.
    - Then, install required libraries:
    ```bash
    pip install -r requirements.txt
    ```

5. **Set up environment variables:**
    - Create a `.env` file in the project root directory to store API keys and configurations.
    - Add your API keys and any other required configurations. For example:
      ```plaintext
      TAVILY_API_KEY=your_api_key_here
      ```
    - Make sure to replace `your_api_key_here` with your actual API key from Tavily or any other service.

6. **Run the application:**
    ```bash
    python app.py
    ```

    - The server will start, and you should see a message indicating that the application is running.
    - Open your browser and navigate to `http://localhost:3000` to access the frontend.

## Roadmap / Todo

- [x] Add Smooth Scrolling
- [ ] Add User Support (Login Pages, MySQL backend, Custom User Pages)
- [ ] Host the Server (on AWS or Heroku)
- [x] Integrate Tavily API for Real-time Data Fetching
- [ ] Implement Personalized Itinerary Generation Logic
- [ ] Add Planner Critique and Feedback System
- [ ] Optimize Agent Communication for Faster Query Processing
- [ ] Create User Dashboard for Itinerary Management
- [ ] Implement Multi-lingual Support for Global Users
- [ ] Add Budget Optimization Feature for Cost-efficient Itineraries
- [ ] Improve Mobile Responsiveness for Seamless Experience on All Devices
- [ ] Integrate Third-party Services (e.g., Booking.com, Google Maps)

## Contributing

Contributions are welcome! To get started:

1. Fork the repository.
2. Create a new branch:
    ```bash
    git checkout -b feature-branch-name
    ```
3. Make your changes and commit them:
    ```bash
    git commit -m "Add some feature"
    ```
4. Push to the branch:
    ```bash
    git push origin feature-branch-name
    ```
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
