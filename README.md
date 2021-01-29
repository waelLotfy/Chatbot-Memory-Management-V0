# Chatbot-Memory-Management-
based on Modern C++ 

This project is able to discuss some memory management topics based on the content of a knowledge base stored in a text file.

I have optimized the project from a memory management perspective using memory concepts in modern C++.

This project is based on udacity C++ nanodegree program.

# Added features

Task 1 : Exclusive Ownership 1 :
In file chatgui.h / chatgui.cpp, make _chatLogic an exclusive resource to class ChatbotPanelDialog using an appropriate smart pointer. Where required, make changes to the code such that data structures and function parameters reflect the new structure.

Task 2 : The Rule Of Five :
In file chatbot.h / chatbot.cpp, make changes to the class ChatBot such that it complies with the Rule of Five. Make sure to properly allocate / deallocate memory resources on the heap and also copy member data where it makes sense to you. In each of the methods (e.g. the copy constructor), print a string of the type „ChatBot Copy Constructor“ to the console so that you can see which method is called in later examples.

Task 3 : Exclusive Ownership 2 :
In file chatlogic.h / chatlogic.cpp, adapt the vector _nodes in a way that the instances of GraphNodes to which the vector elements refer are exclusively owned by the class ChatLogic. Use an appropriate type of smart pointer to achieve this. Where required, make changes to the code such that data structures and function parameters reflect the changes. When passing the GraphNode instances to functions, make sure to not transfer ownership and try to contain the changes to class ChatLogic where possible.

Task 4 : Moving Smart Pointers :
In files chatlogic.h / chatlogic.cpp and graphnodes.h / graphnodes.cpp change the ownership of all instances of GraphEdge in a way such that each instance of GraphNode exclusively owns the outgoing GraphEdges and holds non-owning references to incoming GraphEdges. Use appropriate smart pointers and where required, make changes to the code such that data structures and function parameters reflect the changes. When transferring ownership from class ChatLogic, where all instances of GraphEdge are created, into instances of GraphNode, make sure to use move semantics.

Task 5 : Moving the ChatBot :
In file chatlogic.cpp, create a local ChatBot instance on the stack at the bottom of function LoadAnswerGraphFromFile. Then, use move semantics to pass the ChatBot instance into the root node. Make sure that ChatLogic has no ownership relation to the ChatBot instance and thus is no longer responsible for memory allocation and deallocation. Note that the member _chatBot remains so it can be used as a communication handle between GUI and ChatBot instance. Make all required changes in files chatlogic.h / chatlogic.cpp and graphnode.h / graphnode.cpp. When the program is executed, messages on which part of the Rule of Five components of ChatBot is called should be printed to the console.

