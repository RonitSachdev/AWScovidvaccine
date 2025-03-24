# COVID-19 Vaccination Center Finder

## Overview
This is a web application that helps users find the nearest COVID-19 vaccination center based on their entered PIN code. It provides real-time information about availability, vaccine types, and slots. The website is hosted using AWS Elastic Beanstalk for scalability and ease of deployment.

## Features
- **Search by PIN Code**: Enter your postal PIN code to find nearby vaccination centers.
- **Real-Time Availability**: Fetches up-to-date vaccine slot availability.
- **Vaccine Type Information**: Displays the available vaccine brands.
- **User-Friendly Interface**: Simple and clean UI for easy navigation.
- **Hosted on AWS Elastic Beanstalk**: Ensures reliable performance and scalability.

## Tech Stack
- **Frontend**: HTML, CSS, JavaScript (React/Vanilla JS)
- **Backend**: Node.js (Express) / Python (Flask/Django)
- **Database**: PostgreSQL / MySQL / DynamoDB (if applicable)
- **Hosting**: AWS Elastic Beanstalk
- **API**: Uses government/public APIs for vaccine availability data

## Deployment on AWS Elastic Beanstalk
To deploy this application on AWS Elastic Beanstalk:

1. **Install AWS CLI and Elastic Beanstalk CLI**:
   ```sh
   pip install awsebcli --upgrade --user
   ```
2. **Initialize Elastic Beanstalk application**:
   ```sh
   eb init -p <platform-name> my-vaccine-finder
   ```
3. **Create an environment and deploy**:
   ```sh
   eb create vaccine-finder-env
   eb deploy
   ```
4. **Monitor the application**:
   ```sh
   eb status
   eb logs
   ```

## Setup and Usage
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/vaccine-finder.git
   cd vaccine-finder
   ```
2. Install dependencies:
   ```sh
   npm install  # If using Node.js
   pip install -r requirements.txt  # If using Python
   ```
3. Start the server:
   ```sh
   npm start  # For Node.js
   python app.py  # For Python
   ```
4. Open the browser and visit:
   ```
   http://localhost:3000  # Adjust the port if necessary
   ```

## Environment Variables
Make sure to configure the following environment variables:
```
API_KEY=your-public-api-key
DATABASE_URL=your-database-url
AWS_ACCESS_KEY_ID=your-aws-key
AWS_SECRET_ACCESS_KEY=your-aws-secret
```

## Future Enhancements
- Add map integration to visualize nearby centers.
- Implement user authentication for appointment booking.
- Support for multiple languages.

## License
This project is licensed under the MIT License.

---

Developed with ❤️ to help people find vaccination centers easily!
