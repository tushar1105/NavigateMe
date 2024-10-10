# READ-ME: Navigate Me iOS App - Tushar Sharma

## Application Overview

    - The application aims to provide the user with directions from a source to a destination location along with some additional details like distance, source and destination coordinates.
    
    - The application seeks for user's permission to begin tracking the location, and when the user allows for the same, the application points to the current location of the user.
    
    - I have added an additional field to display the time taken for the journey to make it more informative for the user.
    
    - The user can toggle between various modes of transport to decide on the route and all display values change dynamically.
    
    - A slider has been provided to allow the user to smoothly zoom in and out of the map for better usability.
    
    - A reset button is added to allow the user to put the application back to its original state.
    
    - The application provides descriptive alert messages to the user informing about the system responses based on his actions.

    - For greater code readability, the code files are organised into logical folders namely - View, Controller and Utilities and class files contain descriptive comments for the functionality of modules and references if any.

## Application Structure
    
### View
    - LaunchScreen: The first screen displayed when the application is launched.
    - Main: A map view, along with various action buttons and outlets.

### Controller
    - ViewController: The main controller for the map view and the related actions.
        - implements the CLLocationManagerDelegate and MKMapViewDelegate from the CoreLocation and MapKit packages respectively required for navigation.
        
## Key learning outcomes for me from the task

- Succesfull implementaion of GPS and Maps in an app to allow navigation.
- Implementing CLGeocoder() which converts a text into the corresponding coordinates out of the box.
    - also, it is an Asynchronous method which means that its execution is independent and on a different thread to that of the main application, executing it successfully was a challenge.
- Learnt about the Dispatch queue and how multithreading is implemented in the app, for the changes to be reflected in the main UI everything has to be synchronised to work on the main thread.

### Note: I tested the app with the various location options available in the simulator like custom and apple, including the city run, bicycle ride and freeway ride and obeserved the location coordinates updated dynamically.

### However, the transit mode did not return any routes even when tested with locations which have an exsting transit system, the problem could not be resolved.
    
        
        
