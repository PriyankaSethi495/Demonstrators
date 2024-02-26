# Projects

# 1. 1st Demonstrator
**Problem:**
The task involved developing a frontend web application for the first demonstrator project, which aimed to enable users to find similar components of a vehicle's components based on uploaded 3D files. The project relied on an existing backend that computed similarities between parts using a method like Euclidean Distance.

The challenge was to create an intuitive user interface that allowed users to upload 3D files, select a computation method, compute similar components, and visualize the results effectively. Additionally, the application needed to facilitate side-by-side comparison of selected and similar components and provide detailed analysis through histogram-based graphs.

**Resolution:**
To address the requirements of the project, a combination of Flask for the backend server and React.js for the frontend web application was employed. This choice allowed for seamless communication between the frontend and existing backend while providing a responsive and interactive user interface.

The frontend application was designed to start with users uploading STL files, which were then rendered using an STL viewer component for visualization. Users could select the desired computation method and initiate the similarity computation process. This involved making requests to the Flask server, which retrieved similar components from the backend based on the uploaded 3D file and computation method.

The retrieved similar components were presented to users as a list along with their similarity scores, allowing for easy comparison. Users could then view these similar parts in a separate viewer and compare them side by side with the selected component.

To provide a detailed analysis of the technical aspects of the components, a chart component was implemented to visualize histogram-based graphs for both the selected component and its similar counterparts. This feature enabled users to gain insights into the similarities and differences between components at a glance, aiding in informed decision-making.

**Approach:**
The development approach for the project involved the following steps:
1. **Requirement Understanding:** Thoroughly analyzing the project requirements, including the need for 3D file uploading, computation method selection, similarity computation, result visualization, and histogram-based analysis.
2. **Technology Selection:** Choosing Flask for the backend server to interface with the existing backend and React.js for the frontend to ensure a dynamic and responsive user interface.
3. **Component Design:** Designing modular React components to handle various aspects of the application, such as file uploading, React STL Viewer for interactive file visualization, computation initiation, result presentation, side-by-side comparison, and React Graph Component for interactive histogram-based analysis.
4. **Integration:** Integrating the frontend and backend components to enable seamless communication and data exchange, ensuring smooth operation of the application.
5. **Testing and Optimization:** Conducting thorough testing to identify and rectify any issues or bugs, optimizing the application for performance and usability.

By following this structured approach, a frontend web application for the project was successfully developed, enabling users to efficiently find similar components of vehicle parts and perform detailed technical analysis through histogram-based graphs.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 2. 2nd Demonstrator
**Problem:**
The task at hand was to develop a frontend web application for the second Demonstrator project. This application needed to depict a pilot project aimed at predicting faults in vehicle components using Artificial Intelligence (AI) and Machine Learning (ML) techniques, leveraging historical data. The primary goal was to create an intuitive interface that could display fault codes retrieved from connected vehicles, along with detailed information about the faulty components, their causes, effects, and countermeasures. Additionally, the application required the capability to predict faults in various car types, each identified by unique car IDs and names, and to present fault details categorized as critical, warning, and informational.

**Resolution:**
To address this challenge, the development of a React-based web application was initiated. This choice was made due to React's flexibility, component-based architecture, and robust ecosystem, which suited the project requirements well. Leveraging React's component model, reusable components were designed for displaying fault codes and their associated details in collapsible accordions, categorized by severity. Each accordion panel provided comprehensive information about the fault, including the reason behind the fault code and suggestions for rectification.

In addition to fault code visualization, a Sankey diagram was implemented to visually represent the relationships between faults and their corresponding vehicle parts. This diagram served as an intuitive tool for users to grasp the interconnectedness of faults and identify potential root causes more effectively.

**Approach:**
To accomplish the development tasks efficiently, a structured approach was followed:
1. **Requirement Analysis:** Thoroughly understanding the project requirements, including the vehicle details and fault code visualization, and detailed fault information presentation.
2. **Technology Selection:** After evaluating various frontend frameworks, React.js was chosen due to its suitability for building interactive user interfaces and managing complex state logic.
3. **Component Design:** Modular React components were designed to encapsulate distinct UI elements, such as fault code displays, accordion panels, and the Sankey diagram, ensuring reusability and maintainability.
4. **Data Management:** State management techniques, including local state and context dummy API, were implemented to efficiently manage and propagate data throughout the application.
5. **Visualization:** Visualization libraries like React Google Charts were employed for creating an interactive Sankey diagram and ensuring clear and insightful fault representation.

By following this systematic approach, a frontend web application was successfully developed that met the project requirements, effectively showcasing the capabilities of the Demonstrator in predicting and managing vehicle faults.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 3. Microsoft Azure Cloud Services: 
**Problem:**
The project requirement involved creating a web interface to manage user databases and blob storage containers using Microsoft Azure services. This included implementing CRUD (Create, Read, Update, Delete) operations for user management in a NoSQL database and file management in blob storage. The task also included setting up resources in the Azure portal, such as databases for user management and blob storage for file management. Additionally, Azure Functions were required to serve as HTTP trigger endpoints for handling CRUD operations.

For user management, CRUD operations included viewing user details, adding users, removing users, and updating user information. For blob storage file management, operations included viewing containers, adding containers, deleting containers, and managing files within containers (viewing, adding, deleting). Furthermore, there was a need to update a CSV file with metadata whenever files were uploaded or deleted, requiring the use of additional functions.

Subsequently, a frontend application was to be developed to provide a user interface for accessing and utilizing these functionalities. The application was expected to begin with a login page, followed by the ability for authenticated users to switch between user management and database management sections to perform their respective operations using HTTP requests and responses from the defined endpoints.

**Resolution:**
To address these requirements, the project proceeded with the following steps:
1. **Azure Resource Setup:** In the Azure portal, a resource group was created containing necessary resources such as NoSQL databases for user management and blob storage for file management.
2. **Azure Functions Development:** Azure Functions were developed to serve as HTTP trigger endpoints for handling CRUD operations for both user management and blob storage file management. These functions were designed to interact with the respective Azure services to perform the required operations.
3. **CSV File Update Function:** An additional Azure Function was created to update a CSV file with metadata whenever files were uploaded or deleted in the blob storage containers.
4. **React Frontend Implementation:** A React-based frontend application was developed to provide a user-friendly interface for accessing the CRUD functionalities. The application included a login page for authentication and separate sections for user management and database management, allowing users to perform operations through HTTP requests to the Azure Functions endpoints.

By following this approach, the project successfully met the requirements of managing user databases and blob storage containers using Microsoft Azure services. The combination of Azure Functions for backend logic and a React frontend for user interaction provided a comprehensive solution for effective database and file management through a web interface.   

--------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 4. Neo4j graph database and recommendation system:
**Problem:**
The project required the integration of a Neo4j graph database and a recommendation system to facilitate efficient search and recommendation functionalities based on user input. Specifically, the project aimed to display components based on user search queries, necessitating the use of Neo4j for CRUD (Create, Read, Update, Delete) operations on sheets stored in CSV files, along with their associated metadata and values. Additionally, the project required the implementation of a basic recommendation system to provide users with relevant suggestions.

**Resolution:**
To address these requirements, the following steps were undertaken:
1. **Neo4j Graph Database Setup:** A Neo4j graph database was set up to store and manage data extracted from CSV files. This involved creating nodes and relationships within the graph to represent the data structure effectively.
2. **CRUD Operations Script:** A script was developed to perform CRUD operations on the Neo4j graph database using the Neo4j driver. This script included functionality to connect to the Neo4j database, load data from CSV files into the graph as nodes and relationships, and implement functions for CRUD operations such as adding, retrieving, updating, and deleting data.
3. **Recommendation System Implementation:** For the recommendation system (since the project was new-basic content-based filtering was implemented), the Neo4j graph database was utilized to leverage indirect relationships between nodes for making recommendations. By analyzing the graph structure and traversing relationships, the recommendation system generated suggestions based on similarities or associations between components.
4. **Integration with Frontend:** The CRUD operations script and recommendation system functionality were integrated into the frontend application. User input from search queries was processed, and relevant data was retrieved from the Neo4j graph database to display matching components. Additionally, recommendations generated by the recommendation system were presented to users based on their interactions with the application.

Through the integration of a Neo4j graph database and a recommendation system, the project successfully addressed the requirement to display components based on user search queries and provide relevant recommendations. The use of Neo4j facilitated efficient CRUD operations on data stored in CSV files, while the recommendation system utilized the graph structure to offer personalized suggestions to users. Overall, the project achieved its objectives of enhancing user experience through effective data management and recommendation functionalities.
