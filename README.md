# Pico-CTF-Challenge-It-is-my-birthday.


![image](https://github.com/user-attachments/assets/bad70f33-23bd-4538-b508-2fcb97f257b0)

## Objective
The goal of this project is to solve the “It is my Birthday” challenge from picoCTF by analyzing patterns in date formatting, logic-based constraints, and HTTP request behavior. This challenge tests the participant’s ability to think critically about how web servers process form inputs or headers, particularly around date-based access restrictions. The objective is to identify the correct format and value that bypasses a restricted input validation to gain access or retrieve the hidden flag.



##🧠 Skills Learned

- Vulnerability scanning and fingerprinting Windows services

- Identifying RCE vectors via HTTP request injection or file parsing flaws

- Payload crafting and testing for remote execution

- Privilege escalation on Windows systems

- Using Metasploit for auxiliary scanning and exploitation

- Leveraging PowerShell for post-exploitation

- Analyzing network traffic with Wireshark to trace exploit behavior

### 🛠️ Tools Used

- Wget - Identification of target  URL and testing  connectivity

- Burp Suite – For HTTP request manipulation

- picoCTF platform – For the challenge environment

- Browser DevTools – For inspecting headers and debugging the form behavior

🧱 Step-by-Step Attack Summary

-  I visited Visit the provided URL for the "It is my birthday" challenge.

  ![image](https://github.com/user-attachments/assets/9fae348f-5599-4d23-80a9-9cff9c1c7410)


-  I used my browser's developer tools (by right-clicking the page and select "Inspect" or press F12) to examine the HTML and JavaScript code of the webpage. Look for clues, comments, hidden fields, or JavaScript functions that might be relevant to the challenge.

  ![image](https://github.com/user-attachments/assets/e3bdf455-6ab1-422d-929e-7ff3feb4c8b6)


- I Used wget to connect to the challenge host and inspect headers and responses to verify server availability.

![image](https://github.com/user-attachments/assets/78d7ea88-4e2c-4cc5-a5d3-28ee4843b59b)
  

- I analyzed the request to check If there is a form or an input field on the page, I tried submitting different values and observe the requests using tools like Burp Suite or the browser's network tab in developer tools and pay attention to any parameters being sent.

  ![image](https://github.com/user-attachments/assets/a4899a66-a0ea-47d3-b5f8-f1b796d33487)



- Flag RetrievalNavigated through user directories or specified challenge paths to locate and extract the flag.

![image](https://github.com/user-attachments/assets/dfa10dd0-7bbc-4bd6-b913-57d012bac9ee)

- I search for common vulnerabilities such as SQL injection, cross-site scripting (XSS), or logic flaws that could be exploited.

- I crafted a payload to exploit the vulnerability. For example, SQL injection, payload: sql ' OR '1'='1
or if it involves manipulating dates, consider how dates are formatted and processed. And I Use the payload in the relevant input field or request parameter and submit it. I Observed the response and look for the flag.

![image](https://github.com/user-attachments/assets/a99d506c-dbbc-4190-a4dd-b4f08ecabd7d)

- Extract the Flag: Once you have successfully exploited the vulnerability, the flag revealed

  ![image](https://github.com/user-attachments/assets/55d6c993-fe27-46b1-b211-cafb45255cae)




