:warning: This service is still in production.


# Virtual Travel Agent

**Virtual Travel Agent** is designed to simplify vacation planning by generating personalized itineraries based on specific user inputs. The system leverages a multi-agent architecture, where each agent performs a distinct role to ensure a seamless vacation planning experience.

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




## Todo:
- [x] Add Smooth Scrolling
- [ ] Add User Support (with Login Pages, MySQL backend, Custom User pages)
- [ ] Host the Server

