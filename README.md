


# No-BS College Predictor

No-BS College Predictor is a simple, no-nonsense tool that allows JEE aspirants to predict potential colleges based on their ranks. This tool eliminates the need for unnecessary logins, data collection, or spammy experiences found on other platforms. The goal is to provide a clear and fast interface to help students focus on choosing the right college based on their rank, category, and exam type (JEE Mains or Advanced).

## Features
- **Instant College Predictions**: Get accurate predictions based on your rank without any delays.
- **Filter by Category**: Apply filters such as OPEN, OBC, SC/ST categories to narrow down college options.
- **JEE Mains or Advanced**: Toggle between JEE Mains and JEE Advanced to get relevant college predictions.
- **No Data Collection**: No account creation or data harvesting. Your privacy is respected.
- **Fast and Responsive UI**: A clean and responsive user interface built with ReactJS and CSS.

## Technology Stack
- **Frontend**: ReactJS
- **Styling**: CSS (custom styling for responsive and sleek design)
- **Package Management**: npm/yarn
- **Build Tool**: React Scripts

## How It Works
1. Select your exam type (JEE Mains or JEE Advanced).
2. Enter your rank in the input box.
3. Click the "Get Predictions" button to see a list of potential colleges.
4. Apply filters like category to narrow down the college list.
5. The list is dynamically generated based on your inputs and filters.

## Installation

### Prerequisites
Make sure you have **Node.js** and **npm** or **yarn** installed on your machine.

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/2AMDevs/no-bs-college-predictor.git
   ```
2. Navigate to the project folder:
   ```bash
   cd no-bs-college-predictor
   ```
3. Install the dependencies:
   ```bash
   npm install
   ```
   or
   ```bash
   yarn install
   ```
4. Start the development server:
   ```bash
   npm start
   ```
   or
   ```bash
   yarn start
   ```
   The app will be live at `http://localhost:3000`.

## Usage
1. Enter your JEE rank in the input box.
2. Select the exam type (JEE Mains or JEE Advanced).
3. Click "Get Predictions" to see a list of possible colleges.
4. Use filters to refine the college list based on your category and preferences.

## Folder Structure
- **src/components**: Contains reusable React components like `CollegePredictor`, `PredictionTable`, and `TableFilter`.
- **src/css**: Contains all CSS files to style the components.
- **src/utils**: Contains utility functions like fetching data for categories.

## Contributing
Feel free to open issues or submit pull requests if you have any suggestions or improvements. Contributions are always welcome!

## Future Enhancements
- **State Quotas**: Add a feature to filter by state quota.
- **More Exam Support**: Expand support to include other exams like BITSAT, VITEEE.
- **Dynamic Rank Update**: Provide real-time updates based on changes in rank cut-offs.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---
