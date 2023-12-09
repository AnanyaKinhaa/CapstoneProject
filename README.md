# CapstoneProject
## Project Breakdown
**Prework: Sign up for IBM Cloud Lite account and create a Watson Natural Language Understanding service.**

1. Create an IBM Cloud Lite account, if you don’t have one already.
2. Create an instance of the Natural Language Understanding (NLU) service.

**Fork the GitHub repo containing the project template. The main web application is a predefined Django application,
you will need to add some new features then build and run your project implementation.**

1. Fork the repository in your account.
2. Clone the repository in the IBM Skills Network Cloud IDE environment.
3. Create static pages to finish the user stories.
4. Run the application locally.

**Add user management to the Django application.**

1. Implement user management using the Django user authentication system.
2. Set up continuous integration and delivery.
   
**Implement backend services.**

1. Create cloud functions to manage dealers and reviews.
2. Create Django models and views to manage car model and car make.
3. Create Django proxy services and views to integrate dealers, reviews, and cars together.

**Add dynamic pages with Django templates.**

1. Create a page that displays all the dealers.
2. Create a page that displays reviews for a selected dealer.
3. Create a page that lets the end user add a review for a selected dealer.

**Run and test your application**

1. Run your application on Cloud IDE
2. Test the updated application locally

## Solution architecture
The solution will consist of multiple technologies

1. The user interacts with the Django application through a web browser.
2. The Django application handles the user authentication using the SQLite database as the persistance layer.
3. The SQLite database also stores the Car Make and the Car Model data.
4. The dealerships and the reviews are stored in Cloudant, a NoSQL document based database.
5. IBM Cloud functions are used to interface with the Cloudant database to get dealerships, get reviews and post reviews.
6. The Django application talks to the IBM Cloud Functions via a set or proxy services.


