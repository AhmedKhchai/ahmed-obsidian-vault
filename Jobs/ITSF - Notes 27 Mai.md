
# Training
## Technical Test Simulation: Django Web Application Development

#### Overview:
You are tasked with creating a simple Django web application called "RadioNetworkManager". This app will manage information about different radio networks, including basic operations like adding, viewing, and deleting network records. The application should be Dockerized for easy deployment.

#### Requirements:
1. **Django Setup**:
   - Set up a new Django project with a single app called `networks`.
   - Use Django 3 or 4, as specified in the job description.

2. **Model Creation**:
   - Create a Django model `RadioNetwork` with the following fields:
     - `name`: A string representing the name of the network.
     - `country`: A string representing the country the network operates in.
     - `active`: A boolean indicating whether the network is active.
   - Enable admin interface for `RadioNetwork`.

3. **Database Integration**:
   - Set up PostgreSQL as the database backend.
   - Ensure the application is configured to connect to a PostgreSQL database.
   - You can simulate the database setup with Docker if you have Docker installed.

4. **Views and URLs**:
   - Implement views for adding a new network, listing all networks, and deleting a network.
   - Use Django's generic class-based views or function-based views as you see fit.

5. **Templates**:
   - Create simple templates for the views. Ensure that they are functional but minimalistic.

6. **Docker Integration**:
   - Dockerize the Django application. Include a `Dockerfile` and a `docker-compose.yml` if necessary.
   - The `Dockerfile` should set up a Python environment, install dependencies, and start the Django server.

7. **Documentation**:
   - Provide a README.md file explaining how to set up and run the application, including how to build and run the Docker container.

#### Evaluation Criteria:
- Functionality: The application should meet all the specified requirements.
- Code Quality: Code should be clean, well-organized, and properly commented.
- Docker Usage: The application should be easily deployable using Docker.

Let's start by setting up a simple Django project to meet these requirements. Would you like to proceed with creating this simulated project here, step-by-step, or would you like a general guide on how to set this up on your own environment?
