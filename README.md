
# Project Background

To create an agent which queries the database to get answers when asked in simple plain english. No SQL code is needed. 

Adhoc queries from the stakeholders can be reported back to them much quciker than before as the analysts need to write the query but only validate the received answer and then share them.

# Assumptions and Caveats

- n8n application is used as low code bridge linking the agent, database, model and SQL query executor. 

# Thought process

- Create something that the user can chat using natural language.
- Convert the natural language to SQL query.
- Run the query directly in the database and display the results in the chat and provide insights along with the results for complex queries.
- Test it multiple times by giving complex queries.

# Solution Design

- A chat trigger which starts the flow with question in natural language.
- An AI agent that understands the input, plans and executes the final answer. 
- Think of an AI agent has an intern who is given specific task which is input, memory to retain previous chat context and a model which acts like a brain to plan and execute.
- A way for AI to look into the all the tables in the database, understand the database schema and the ability to run the SQL query and fetch the data.

# Outcome

- The user chats with an AI and gets answers from the database.
- The AI handles thinking, querying and explaining.
- Adhoc requests are received much quicker as analysts only validate the answers received and then share them to the stakeholders.

![Outcome](Images/Screenshot%202026-11-16%20005723.png)
![Outcome](Images/Screenshot%202026-11-16%20005745.png)
![Outcome](Images/Screenshot%202026-11-16%20010002.png)