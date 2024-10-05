:warning: This service is still in production.


Virtual-Travel-Agent
Designed to simplify vacation planning by generating personalized itineraries based on specific user inputs.

The architecture of the system consists of multiple interacting agents, each responsible
for a specific aspect of the vacation planning process. The system’s overall flow is as
follows:
• The Vacation Planning Supervisor initializes the process by defining the user’s
preferences and parameters.
• The Planner Assistant generates search queries and pulls data from the Tavily API.
• The Vacation Planner takes the gathered data and constructs the initial itinerary.
• The Planner Critique agent evaluates the itinerary and suggests improvements.
• The Planner Critique Assistant refines the plan by performing additional searches
and incorporating new data into the itinerary.
This structure allows the agents to work in harmony, ensuring a seamless and efficient
vacation planning process. Figure 1 shows the overall architecture of the system.


## Todo:
- [x] Add Smooth Scrolling
- [ ] Add User Support (with Login Pages, MySQL backend, Custom User pages)
- [ ] Host the Server

