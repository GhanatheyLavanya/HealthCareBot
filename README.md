# HealthCareBot
 
**INTRODUCTION**

Having quick and reliable access to information on medical facilities is essential in the healthcare sector. The goal of this project is to create an intuitive system that will enable users to search for and obtain data on healthcare facilities according to their location and facility type. In the current project, a web application built with Flask has been created to give users access to healthcare facility information. To manage user interactions and retrieve data from a preprocessed healthcare dataset, the application makes use of a ChatBot class. Additionally, it will provide important information like insurance acceptance, convenient hours, and emergency service availability. Our mission is to empower clients with the knowledge they need to make wise healthcare decisions. Our main goal is to empower our customers by making essential healthcare information more accessible to all. Beyond just giving people information, our mission encompasses our dedication to empowering people and giving them the knowledge they need to successfully navigate and make decisions in the complex world of healthcare services. One potential path forward for ongoing improvement and development is the incorporation of Language Model-based Learning (LLM) systems. Our ChatBot's capability can be enhanced beyond what it is now capable of by utilizing sophisticated language models, such as those driven by machine learning and natural language processing (NLP). 

**RELATED WORK** 

Many studies have focused on data integrity, privacy, and effective storage while discussing healthcare data management systems. Databases used by these systems frequently hold patient data, hospital information, and medical histories.  A few initiatives have investigated how users can interface with healthcare systems to retrieve information. Web applications and chatbots have been created to help consumers locate healthcare facilities according to their location, the services they need, or their own preferences. Unfortunately, the majority of these systems are only applicable to one hospital or a small number of hospitals, which limits their reach. Our chatbot-driven application interacts with a complete dataset, enabling users to access information across different hospitals and facility types, in contrast to many other existing systems that concentrate on a single hospital or a restricted dataset. Our bot's adaptability is one of its unique features. In contrast to bots that are exclusive to a single hospital, our application compiles data from a variety of healthcare institutions. When consumers seek healthcare providers, this inclusivity gives them access to a wider range of options and information, improving their ability to make choices. 

**METHODOLOGY** 

**1. Flask App Initialization** 

Purpose: The goal of the Flask framework is to create an instance of the Flask class and initialize the web application. 

CORS Integration: To enable communication with the application from many domains, CORS (Cross-Origin Resource Sharing) is used. The server can reply to cross-origin requests if CORS is enabled. 

**2. ChatBot Class**

Role: The application's ChatBot class serves as the foundation for all user interactions. 

Functionality: 

Message Handling: To collect preferences and handle requests, the class methods handle user input by directing users through a conversational flow. 

Dataset Interaction: Based on input supplied by the user, the ChatBot queries and retrieves data from the healthcare dataset. 

Response Generation: Based on user input, it presents appropriate healthcare facility details in response to user communications. 

**3. Data Loading and Processing **

Dataset Source: An Excel file serves as the original source of the data. 

Steps in Preprocessing: The dataset is loaded into a Pandas DataFrame during the loading process. 

Managing Missing Values: Fillna() and other techniques may be used to identify and handle missing values in the dataset. 

Character Standardization: To maintain uniform formatting, special characters are replaced, such as apostrophes. 

Data Consistency: Inconsistencies in formatting (such as trailing or preceding spaces) are corrected to provide consistency. 

Storage: To provide easy retrieval and use within the program, the cleaned dataset is stored as a CSV file. 

****4. Flask Pathways ****

URL Routing: In an application, routes are set up to control various user interactions. 

Functionality: 

Root URL ('/'): This renders 'index.html', which is the user interface's entrance point. 

'/map': Shows a map display, possibly with customization options for the user. 

'/submit_message': Responds to messages from users and forwards them to the ChatBot for analysis. 

'/get_data': Based on user input, retrieves essential medical data. 

**5. HTML Templates **

Interface Design: 'map.html' and 'index.html' are examples of HTML templates designed to provide an easy-to-use interface. 

Goal: 

"index.html": Offers a place for users to engage, probably with input forms for preferences. 

"map.html": Based on user requests, this page shows information on healthcare facilities, possibly on a map interface. 

**Requirements**
Python 3.x
Windows


