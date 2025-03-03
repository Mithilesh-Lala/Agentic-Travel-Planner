# AI Travel Planner

An agentic application that uses the Claude API to help plan trips by coordinating multiple specialized AI agents.

## Features

- **Flight Finder Agent**: Searches for flights between origin and destination for specific dates
- **Hotel Explorer Agent**: Finds suitable accommodations at the destination within budget
- **Attraction Scout Agent**: Discovers interesting places and activities at the destination
- **Trip Summarizer Agent**: Creates a comprehensive trip plan by combining information from all agents

## Setup Instructions

### Prerequisites

- Python 3.8 or higher
- An Anthropic API key (with access to Claude models)

### Installation

1. Clone this repository:
   ```
   git clone https://github.com/Mithilesh-Lala/Agentic-Travel-Planner.git
   cd ai-travel-planner
   ```

2. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

3. Run the application:
   ```
   streamlit run app.py
   ```

4. Open your web browser and navigate to the URL shown in the terminal (typically http://localhost:8501)

### Using the App

1. Enter your Anthropic API key in the sidebar
2. Fill in your trip details:
   - Origin and destination cities
   - Departure and return dates
   - Budget level
   - Number of travelers
   - Interests
3. Click "Plan My Trip"
4. View the results in each tab:
   - Flights
   - Hotels
   - Attractions
   - Complete Trip Plan
5. Download your complete trip plan as a markdown file

## System Architecture

The application uses an agentic approach with four specialized AI agents:

1. **Flight Finder Agent**: Focused on transportation options
2. **Hotel Explorer Agent**: Specialized in finding accommodations
3. **Attraction Scout Agent**: Expert in points of interest and activities
4. **Trip Summarizer Agent**: Combines information from other agents into a cohesive plan

Each agent has a specialized system prompt that guides its responses. The agents run sequentially, and their outputs are combined for the summary agent to create the final trip plan.

## Customization

You can customize the agents' behavior by modifying their system prompts in the code. Each agent has a dedicated system prompt that defines its role and the type of information it should provide.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
