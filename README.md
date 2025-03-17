## Server Reconnection Handler

#### Overview
The Server Reconnection Handler is a simple HTML, CSS, and JavaScript application that attempts to automatically reconnect to an unavailable server and provides a manual reconnection button for users.

#### Features
- Displays a message when the application is not accessible.
- Automatically checks for server availability at set intervals.
- Provides a Reconnect button for manual reconnection attempts.
- Redirects users to the target URL when the server is back online.
- Uses a CSS loading spinner to indicate an ongoing reconnection attempt.

#### Installation & Usage
##### Prerequisites
- A web browser
- A server hosting the application

##### Running the Application
- Download or clone the repository.
- Open index.html in a browser.
- The application will attempt to reconnect automatically.
- Click the Reconnect button to manually attempt reconnection.

##### Configuration
- Modify the following constants in the script section to adjust behavior:
```
const URI = window.location.hash.substring(1); // Target URL
const RECONNECTION_INTERVAL = 5000; // Interval to check URL (milliseconds)
const REDIRECTION_TIME = 0; // Redirection delay
const RECONNECTION_TIME_OUT = 20000; // Timeout duration (milliseconds)
```

#### Code Explanation
HTML Structure
- A centered div containing a message and a reconnect button.
- The button changes its label dynamically based on connection status.

JavaScript Functionality
```
fetchHTTPRequest(uri, redirectionTime): Checks if the target server is reachable.
btnReconnect.onclick: Triggers a manual reconnection attempt.
autoRequest(): Automatically attempts reconnection at intervals.
redirectionCallBack(url): Redirects to the target URL upon successful reconnection.
```

#### CSS Styling
- Basic styling for the reconnect UI.
- A loading spinner to indicate an ongoing reconnection attempt.

#### License
This project is open-source and available under the MIT License.

#### Author
Developed by Bishal Shrestha.

![image](https://github.com/user-attachments/assets/ea13009b-349d-4672-b03f-267eb725f281)

