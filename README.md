# OTP Authentication – Phone Number Verification App

**Requirements**
- A modern web browser (Chrome, Firefox, Edge, Safari)  
- Active internet connection for OTP and verification services  
- A valid **Phone.Email Client ID** configured in the HTML  
- Basic understanding of HTML and JavaScript for integration and customization  
- Backend server (optional but recommended) to securely fetch verified user details  

**Technologies Used**
- **HTML** for structuring the authentication interface  
- **Vanilla JavaScript** for handling verification callbacks and UI updates  
- **Phone.Email OTP Authentication SDK** for phone number verification  
- **Client-side Event Handling** to process authentication success  

**About the Authentication Service**
- **Phone.Email OTP Authentication**
  - Provides passwordless phone number authentication using OTP  
  - Handles OTP sending, verification, and validation securely  
  - On successful verification, returns a `user_json_url`
  - The `user_json_url` can be used by the backend to fetch:
    - Verified phone number  
    - Country code  
    - Authentication metadata  
  - Authentication flow is handled externally, reducing security risks on the client  

**Features Implemented**
- One-click phone number verification using OTP  
- Secure third-party authentication integration  
- Callback listener (`phoneEmailListener`) triggered after successful verification  
- Displays temporary success message for debugging and testing  
- No manual OTP handling required on the frontend  
- Lightweight and minimal setup  

**Application Flow**
- User clicks the **Phone.Email Sign-In** button  
- OTP is sent to the user’s phone number  
- User enters OTP and completes verification  
- On success, `phoneEmailListener` is triggered  
- A `user_json_url` is returned for backend verification  
- Success message is displayed (for development/debug purposes)  

**Notes**
- The displayed success message is meant only for debugging  
- In production, the `user_json_url` should be sent securely to the backend  
- Do not expose sensitive authentication data on the frontend  
- This project demonstrates passwordless authentication integration  

**Possible Enhancements**
- Integrate backend API to securely fetch and store verified phone numbers  
- Redirect users after successful authentication  
- Add session management and logout support  
- Improve UI with loading states and success animations  
- Combine OTP login with other authentication methods  
