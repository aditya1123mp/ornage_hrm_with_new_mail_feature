# OrangeHRM Automation Project

This project is designed to automate several tasks on the OrangeHRM site, including user management and email-based credential handling. The automation involves logging into the site, creating a new employee with randomly generated credentials, sending those credentials via email, retrieving the credentials from another email account, and using them to verify the new user's information.

## Features

- **Login Automation**: Automates the login process to the OrangeHRM site.
- **Employee Management**:
  - Creates a new employee with a randomly generated username and password.
  - Stores the generated credentials in global variables for later use.
- **Email Automation**:
  - Sends the newly generated username and password to a specified email address.
  - Retrieves the credentials from a different email account.
- **User Verification**:
  - Uses the retrieved credentials to log back into the OrangeHRM application.
  - Verifies the information of the newly created user.
- **Profile Picture Update**: Adds a profile picture for the new user using automation.

## Technologies Used

- **Katalon Studio**: For creating and running the automation scripts.
- **Groovy**: Scripting language used within Katalon Studio for custom logic and email handling.
- **JavaMail API**: Used for sending and retrieving emails programmatically.

## Project Structure

- `Test Cases/`: Contains the test cases for each automation scenario, including user creation, email handling, and user verification.
- `Global Variables/`: Stores the global variables, including the randomly generated username and password.
- `Profiles/`: Stores different profiles for different environments, such as development and production.
- `Object Repository/`: Contains the web elements used in the automation scripts.
- `Keywords/`: Custom Groovy scripts used for email sending and retrieval.

## Getting Started

### Prerequisites

- **Katalon Studio**: Ensure you have Katalon Studio installed.
- **JavaMail API**: Make sure the required dependencies for email handling are added to your project.
- **Access to OrangeHRM Site**: Ensure you have access to the OrangeHRM site for testing.
- **Email Accounts**: Set up two email accounts for sending and retrieving credentials.

### Setup

1. Clone this repository to your local machine.
2. Open the project in Katalon Studio.
3. Configure the global variables with your specific data, such as the OrangeHRM site URL, email credentials, and paths for profile pictures.
4. Update the email configurations in the `Keywords/EmailUtils.groovy` file to match your SMTP server and email accounts.

### Running the Tests

1. Open the desired test case from the `Test Cases/` folder.
2. Click the "Run" button in Katalon Studio.
3. The automation script will:
   - Log into the OrangeHRM site.
   - Create a new employee with a randomly generated username and password.
   - Save the credentials in global variables.
   - Send the credentials via email.
   - Retrieve the credentials from another email account.
   - Log in with the retrieved credentials and verify the new user's information.
   - Add a profile picture for the user.

## Customization

- **Credential Generation**: Modify the logic for generating usernames and passwords to meet specific requirements.
- **Email Templates**: Customize the email content sent with the new credentials.
- **User Verification**: Expand the verification process to include additional user details or actions.

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request with your changes, whether they are improvements or new features.

## Contact

For questions, issues, or contributions, please open an issue in the repository or contact the project maintainer.

LinkedIn: www.linkedin.com/in/aditya-agarwal-a291b6146

mail: aditya1993tue@gmail.com

