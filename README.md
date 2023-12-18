# Fuzzy-Bright-Control
Fuzzy Logic Illumination: Navigating Adaptive Brightness Control for Enhanced User Experience

The provided Python code implements a fuzzy logic-based system for controlling brightness levels in a smart lighting scenario. The system takes into account two antecedents, namely ambient light level and user preference level, and outputs a consequent brightness level. Fuzzy logic is employed to model the imprecision and uncertainty inherent in human language, allowing the system to make decisions based on approximate reasoning.

Antecedents and Consequents Definition
The code starts by defining three fuzzy variables: ambient_light, user_preference, and brightness_level. These variables represent the input factors (ambient light and user preference) and the output factor (brightness level), respectively. The universe of discourse for each variable ranges from 0 to 100, and triangular membership functions are assigned to the linguistic terms 'low,' 'medium,' and 'high' for each variable.

Membership Functions
Membership functions define the degree of membership of a value in a linguistic term. In this code, triangular membership functions are used to model the relationships between linguistic terms and their respective variables. The choice of triangular membership functions allows for a simple and intuitive representation of fuzzy sets.

Rules
Three fuzzy rules are defined to capture the relationships between the antecedents and the consequent. These rules are constructed based on linguistic terms and specify how the brightness level should be adjusted based on the combination of ambient light and user preference. The rules use the logical operators 'and' and 'or' to model different scenarios.

Control System and Simulation
The fuzzy control system is defined using the ControlSystem class from the skfuzzy library. This system comprises the fuzzy variables and rules previously defined. Additionally, a ControlSystemSimulation object is created for simulation purposes. This simulation allows for the input of ambient light and user preference levels, computing the corresponding brightness level based on the defined rules and membership functions.

User Input and Output
The user is prompted to input the ambient light level and user preference level. The code then sets these inputs in the simulation and computes the resulting brightness level using the fuzzy logic rules. The computed brightness level is then printed as the output.

Graphical Analysis
The code includes graphical analysis using matplotlib, visualizing the fuzzy sets and their intersections using dot patterns. Three subplots depict the membership functions for ambient light, user preference, and brightness level. This graphical representation provides a visual understanding of how the fuzzy variables interact and influence the output.

Conclusion
In summary, this code demonstrates the implementation of a fuzzy logic-based system for adjusting brightness levels in a smart lighting environment. The use of triangular membership functions and fuzzy rules allows for a flexible and interpretable model that considers both ambient conditions and user preferences. The graphical analysis provides insights into the fuzzy sets' relationships, contributing to a clearer understanding of the decision-making process within the fuzzy control system. This approach exemplifies the application of fuzzy logic in real-world scenarios where precise control is challenging due to imprecise and uncertain input conditions.
