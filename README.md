# CLAAS Demonstrator
**Problem:**
The task involved developing a frontend web application for the CLAAS demonstrator project, which aimed to enable users to find similar components of a vehicle's components based on uploaded 3D STL files. The project relied on an existing backend that computed similarities between parts using a method like Euclidean Distance.

The challenge was to create an intuitive user interface that allowed users to upload 3D STL component, select a computation method, compute similar components, and visualize the results effectively. Additionally, the application needed to facilitate side-by-side comparison of selected and similar components and provide detailed analysis through histogram-based graphs.

**Resolution:**
To address the requirements of the project, a combination of Flask as API for the backend server and React.js for the frontend web application was employed. This choice allowed for seamless communication between the frontend and existing backend while providing a responsive and interactive user interface.

The frontend application was designed to start with users uploading STL files, which were then rendered using an STL viewer component for visualization. Users could select the desired computation method and initiate the similarity computation process. This involved making requests to the Flask API server, which retrieved similar components from the backend based on the uploaded 3D file and computation method.

The retrieved similar components were presented to users as a list along with their similarity scores, allowing for easy comparison. Users could then view these similar parts in a separate viewer and compare them side by side with the selected component.

To provide a detailed analysis of the technical aspects of the components, a chart component was implemented to visualize histogram-based graphs for both the selected component and its similar counterparts. This feature enabled users to gain insights into the similarities and differences between components at a glance, aiding in informed decision-making.

**Approach:**
The development approach for the project involved the following steps:
1. **Requirement Understanding:** Thoroughly analyzing the project requirements, including the need for 3D file uploading, computation method selection, similarity computation, result visualization, and histogram-based analysis.
2. **Technology Selection:** Choosing Flask for the API to interface with the existing backend and React.js for the frontend to ensure a dynamic and responsive user interface.
3. **Component Design:** Designing modular React components to handle various aspects of the application, such as file uploading, React STL Viewer for interactive file visualization, computation initiation, result presentation, side-by-side comparison, and React Graph Component for interactive histogram-based analysis.
4. **Integration:** Integrating the frontend and backend components to enable seamless communication and data exchange, ensuring smooth operation of the application.
5. **Testing and Optimization:** Conducting thorough testing to identify and rectify any issues or bugs, optimizing the application for performance and usability.

By following this structured approach, a frontend web application for the project was successfully developed, enabling users to efficiently find similar components of vehicle parts and perform detailed technical analysis through histogram-based graphs.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Hella Gutmann Demonstrator
**Problem:**
The task at hand was to develop a frontend web application for this Demonstrator project. This application needed to depict a pilot project aimed at predicting faults in vehicle components using Artificial Intelligence (AI) and Machine Learning (ML) techniques, leveraging historical data. The primary goal was to create an intuitive interface that could display fault codes retrieved from connected vehicles, along with detailed information about the faulty components, their causes, effects, and countermeasures. Additionally, the application required the capability to predict faults in various car types, each identified by unique car IDs and names, and to present fault details categorized as critical, warning, and informational.

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


(**Note:** Due to organization's confidentiality, the project code and screenshots cannot be uploaded to GitHub.)
