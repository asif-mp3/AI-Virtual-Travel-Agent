:warning: This service is still in production.

# AI-Virtual Travel Agent

**AI-Virtual Travel Agent** is designed to simplify vacation planning by generating personalized itineraries based on specific user inputs. The system leverages a multi-agent architecture, where each agent performs a distinct role to ensure a seamless vacation planning experience.

## System Architecture

The architecture consists of multiple interacting agents, each responsible for a specific aspect of the vacation planning process. Below is the detailed flow:

1. **Vacation Planning Supervisor**
   - Initializes the planning process by defining the user’s preferences and parameters.
   - Ensures that all the user requirements are understood before further steps are taken.

2. **Planner Assistant**
   - Generates search queries based on the user inputs provided by the Supervisor.
   - Pulls relevant vacation-related data from the **Tavily API** (e.g., places to visit, accommodations, activities).

3. **Vacation Planner**
   - Takes the data gathered by the Planner Assistant.
   - Constructs the initial version of the vacation itinerary based on the user’s preferences and available data.

4. **Planner Critique Agent**
   - Evaluates the generated itinerary.
   - Provides suggestions for improvements, identifying gaps or better alternatives.

5. **Planner Critique Assistant**
   - Refines the initial plan by performing additional searches based on the feedback from the Critique Agent.
   - Incorporates new or improved data into the itinerary for a more polished plan.

This multi-agent architecture allows the system to work efficiently, delivering a customized and well-optimized vacation itinerary tailored to the user’s preferences.

### Additional Features
- **Real-time Data Integration**: The system pulls live data from multiple sources like travel agencies, accommodation providers, and tourism platforms using the **Tavily API**.
- **Feedback Loop**: Continuous feedback from the Planner Critique Agent ensures that the final itinerary is iteratively improved to meet the user's specific requirements.
- **Customization**: The system offers personalized itineraries that can include anything from adventure activities to family-friendly experiences based on the user’s preferences.
- **Seamless User Interface**: A smooth, user-friendly interface ensures that vacation planning is hassle-free.

## Technology Stack

- **Frontend**: HTML, CSS, JavaScript (with smooth scrolling for a better user experience)
- **Backend**: Node.js, Express
- **Database**: MySQL (for user support and itinerary storage)
- **API**: Tavily API for real-time travel data fetching
- **AI Agents**: Built using Python for handling logic, data processing, and itinerary evaluation
- **Hosting**: Planned deployment on AWS or Heroku

## Todo:

- [x] Add Smooth Scrolling
- [ ] Add User Support (with Login Pages, MySQL backend, Custom User pages)
- [ ] Host the Server
- [x] Integrate Tavily API for Real-time Data Fetching
- [ ] Implement Personalized Itinerary Generation Logic
- [ ] Add Planner Critique and Feedback System
- [ ] Optimize Agent Communication for Faster Query Processing
- [ ] Create User Dashboard for Itinerary Management
- [ ] Implement Multi-lingual Support for Global Users
- [ ] Add Budget Optimization Feature for Cost-efficient Itineraries
- [ ] Improve Mobile Responsiveness for Seamless Experience on All Devices
- [ ] Integrate Third-party Services (e.g., Booking.com, Google Maps)

## How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/asif-mp3/AI-Virtual-Travel-Agent.git

2. Navigate into the project directory:
   ```bash
   cd AI-Virtual-Travel-Agent
3. Install the required dependencies:
   - Make sure you have Python and pip installed on your machine. If not, download and install them from the [official Python website](https://www.python.org/downloads/).
   - Install the necessary libraries by running:
   ```bash
   pip install -r requirements.txt
4. Set up environment variables:
   - Create a `.env` file in the project root directory. This file will store your API keys and other configurations securely.
   - Add your API keys and configurations as needed. For example:
     ```plaintext
     TAVILY_API_KEY=your_api_key_here
     ```
   - Ensure you replace `your_api_key_here` with your actual API key from the Tavily API or any other services you are using.
5. Run the application:
   - Start the application by executing the following command:
     ```bash
     python app.py
     ```
   - This will launch the server, and you should see output indicating that the application is running.

