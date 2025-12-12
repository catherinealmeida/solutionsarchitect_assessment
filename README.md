README HubSpot + Demo App

# Introduction

A Node.js demo integrating Breezy e-commerce/thermostat customer data with HubSpot CRM, featuring AI-generated sales prompts and streamlined contact/deal management for sales and marketing teams.

A. Setup Instructions:


- The app was created via VSC + NODE: 
1. Clone repo
2. Install dependencies: `npm install`
3. Create `.env` file (see `.env.sample`)
4. Run with `node server.js`
5. Open `index.html` for frontend usage

HubSpot ID:147416976

- Prerequisites:
1. Node.js vXX
2. HubSpot API key (add to .env)
3. OpenAI API key (add to .env)

- The backend functionalities were cloned from a GitHub repository (changes were added to suit the project)
- The app should be used in a local server to fetch contacts and Deals from the HubSpot portal.
- From the front end (index.html) you can view existing contacts, trials, subscriptions (sample data) and create new contacts and new deals to associate with existing contacts in a HubSpot portal
- OPENAI is added to the server with prompts (*still need further adjustments)
- The following libraries were installed via node.js + vsc:  
 > express,cors, axios, node-fetch,openai, dotenv

B.Project Overview

This project demonstrates how a system can integrate data with HubSpot via API in a straightforward and user-friendly manner. It is designed for non-technical users, allowing them to easily view all HubSpot contacts and deals in a readable table format, and to add new contacts or deals simply by filling out a form. The application provides Sales and Marketing teams with convenient access to review and update HubSpot data.

OpenAI functionality is integrated to assist with drafting email and call summaries, as well as to help Sales and Marketing teams generate customer messages, gather deal details, and support automation and sales strategies.

C. AI Usage Documentation

- ChatGPT was utilized throughout this project.
- It assisted in optimizing code, troubleshooting issues, and designing the script logic to ensure data displayed correctly on the frontend.
- Through this process, I gained experience integrating AI into an application and learned how to use the frontend to display API data with a focus on the customer case goal.


D. HubSpot Data Architecture

ERD - https://lucid.app/lucidchart/f14be198-d619-4144-a59b-2ba80e5b13a6/edit?viewport_loc=-1280%2C-2080%2C6652%2C3124%2C0_0&invitationId=inv_ab87ff37-d845-45ef-b7bf-9fbaff310aad

For the ERD, I focused on the core HubSpot objects necessary to achieve Breezy’s business goals and keep data clear and easy to manage: Contact, Company, and Deal, with an emphasis on B2C sales. Contacts serve as the primary link for automations such as marketing emails, surveys, and sequences, while Deals are used to track customer purchase behavior and associate sales activities between the objects. 
The Deal pipeline can be structured to support two distinct business objectives:

Pipeline 1: Default (Sales Pipeline) for Subscriptions
Pipeline 2: Trials

- Hardware Products can be added as HubSpot products and be used in line items/ quotes
- Payment and quotes can also be used for Products and Subscriptions.

To follow data in HubSpot:
- The Sales team can generate reports based on the Deal pipeline, enabling them to monitor contacts in either the trial or sales stages for commercial and marketing strategies.
- Deal reports based can also be used to calculate the total amount spent by a specific contact. Additionally, analyzing products within line items provides valuable insights into customer behavior. 


E. AI Feature Explanation

- OpenAI was selected for its robust features and ease of integration into the project. In this customer scenario, OpenAI can be leveraged to analyze deal statuses, review contact purchase history, and suggest relevant products. Additionally, the AI can assist with drafting emails, call summaries, messages, and providing real-time chat support.

These functionalities enable the Sales and Marketing teams to optimize campaign creation, efficiently answer customer FAQs, and support personalized communications such as one-to-one emails and call preparations. Overall, AI helps streamline workflows, reduce communication barriers, and keep data up to date, ensuring teams are aligned and better equipped to understand and serve their customers—ultimately driving increased sales.

F. Design Decisions
- I chose to combine HTML and script within each file to speed up development, keeping each file focused on a single function. This approach made it easier to manage and update the code, as any new script or functionality could be added directly within the relevant file.
Given more time, I would further enhance the AI features, improve the application’s styling, and add additional functionalities to deliver even greater value for the customer.

