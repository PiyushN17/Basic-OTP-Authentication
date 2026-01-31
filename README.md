# OTP Authentication – Phone Number Verification App

**Requirements**
- Modern web browser (Chrome, Firefox, Edge, Safari)  
- Internet connection for OTP verification  
- Valid **Phone.Email Client ID**  
- Basic HTML and JavaScript knowledge  
- Backend server (optional, recommended for production)  

**Technologies Used**
- **HTML** for UI structure  
- **Vanilla JavaScript** for handling authentication callbacks  
- **Phone.Email OTP Authentication SDK** for phone verification  

**About the Authentication Service**
- Uses **Phone.Email** for passwordless OTP-based phone authentication  
- Automatically handles OTP sending and verification  
- Returns a `user_json_url` on successful verification for backend processing  

**Features Implemented**
- One-click OTP-based phone number verification  
- Secure third-party authentication integration  
- Callback-based success handling  
- No manual OTP logic on the frontend  

**Application Flow**
- User clicks the Phone.Email sign-in button  
- OTP is sent and verified  
- Success callback returns verification data URL  

**Notes**
- Debug message is for development only  
- In production, verification data should be handled on the backend  

**Possible Enhancements**
- Backend integration for user management  
- Redirect after successful login  
- Add session handling  
