## Flask Application Design: Car Details App

### HTML Files

1. **index.html**: This is the main HTML file that serves as the user interface of the application. It should contain a user-friendly form where users can input their queries about car details in India. The form can include elements like text fields for car models, radio buttons for fuel types, and a submit button.

2. **results.html**: This HTML file is responsible for displaying the results of the user's query. It should contain a neatly formatted table or list to present the car details, including information such as car names, prices, mileage, and fuel efficiency.

### Routes

1. **Homepage Route (/)**: This is the route for the homepage of the application. When a user opens the application, this route should be triggered, rendering the `index.html` file.

2. **Search Route (/search)**: This route handles the user's search query. When the user submits the form on the homepage, this route should be called. It should process the user's input and retrieve the relevant car details from a database or API. After processing, it should render the `results.html` file, passing the retrieved car details to display.

3. **About Route (/about)**: This route displays information about the application, such as its purpose, creators, and any other relevant details. It can be accessed by a dedicated link on the homepage or through the application's navigation system.

4. **Contact Route (/contact)**: This route provides a means for users to contact the application's creators. It should display a form where users can input their names, email addresses, and messages. Upon submission, the form data should be sent to the application's maintainers or stored in a database for later retrieval.

### Application Structure

```
├── app.py
├── templates
│   ├── index.html
│   ├── results.html
│   └── about.html
├── static
│   ├── css
│   │   └── style.css
│   └── images
│       └── logo.png
```