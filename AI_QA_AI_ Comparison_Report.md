# AI_QA_AI_Comparison_Report
**Tester:** QA Engineer
**Date:** 2026-04-16
**Type:** AI Comparative Analysis- ChatGPT vs CodeGPT vs Other AI Tools

## 4.1 API Test Generation

### ChatGPT Output - Login API Test
 
 ## 1. Positive Test Cases
- Valid username and valid password → login successful
- Valid email and correct password → login successful
- Login with remember-me option enabled → session persists
- Login using correct credentials after logout → successful login
- Login with valid credentials across supported browsers → successful

 ## 2. Negative Test Cases
- Invalid username + valid password → login failed
- Valid username + invalid password → login failed
- Empty username and password → validation error
- SQL injection attempt in username field → login blocked
- Special characters in password field with invalid credentials → login failed

 ## 3. Edge Cases
- Very long username/password (1000+ characters)
- Username with spaces at beginning/end
- Case sensitivity check in username/email
- Multiple rapid login attempts (rate limiting trigger)
- Login with expired account credentials

## 4. Security Test Cases
- SQL injection attempts in login fields
- XSS injection in username field
- Brute force attack simulation (multiple failed logins)
- Account lockout after repeated failed attempts
- Password transmission over secure HTTPS only
- Session hijacking attempt after login
- Token expiration validation (JWT/session tokens)

### CodeGPT Output - Login API Test Cases

#### Observed Behavior
- Authentication successful via Google login
- Chat interface blocked by paywall modal
- No test case generation possible due to access restriction

---

### Impact / Key Limitation
- Freemium paywall blocks core AI chat functionality after login, preventing test case generation and workflow continuation.
- Limits usability for end-to-end QA testing in the free tier and disrupts comparative analysis workflows.

### CodeGPT Result – Status

## 1. Positive Test Cases
- Not executed due to UI blocking issue

## 2. Negative Test Cases
- Not accessible due to paywall modal blocking input

## 3.  Edge Cases
- Authentication successful but chat functionality unavailable

## 4. Security / Access Behavior
- User session valid but feature access restricted without credit purchase


## Comparison Impact (Preliminary)
- ChatGPT: Fully functional and responsive 
- CodeGPT: Authenticated but workflow blocked 

## 5. Key Findings
- ChatGPT provided complete, structured, and well-categorized test cases with strong coverage across positive, negative, edge, and security scenarios.
- CodeGPT successfully authenticated but failed to support continuous workflow execution due to a persistent paywall restriction blocking the chat interface.
- ChatGPT demonstrated higher usability and consistent structured output for QA test generation tasks.
- CodeGPT showed limitations in free-tier usability, impacting its effectiveness for full QA workflow testing.
- Both tools can generate QA-related outputs, but only ChatGPT supported uninterrupted testing flow in this evaluation.

## 6. Overall Evaluation
Based on this comparative analysis:

- ChatGPT is more suitable for QA test generation due to complete output consistency, structured responses, and uninterrupted workflow support.
- CodeGPT demonstrates potential in AI-assisted development but is limited by freemium restrictions that block full functionality during testing.

### Final Rating (QA Perspective):
- ChatGPT: 9/10 (Strong structured QA output)
- CodeGPT: 5/10 (Functional but workflow-limited in free tier)

## 7. Skills Demonstrated
- AI Tool Evaluation
- Comparative QA Analysis
- Test Case Design (Positive, Negative, Edge, Security)
- Exploratory Testing
- Usability & Workflow Analysis
- Defect Identification (UI/UX Blocking Issue)
- Technical Documentation in Markdown

