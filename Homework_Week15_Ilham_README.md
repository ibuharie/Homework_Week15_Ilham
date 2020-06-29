## Unit 15 Homework: Web Vulnerabilities and Hardening
Please include the Screenshots folder in the same directory as this markdown file to view the screenshots.
### Overview

This week, you continued your journey towards enhancing your technical acuity through a deeper understanding of web vulnerabilities and system hardening used to help protect and defend critical web infrastructure.

- The homework is divided into two parts:

   - Part 1: Conceptual based Q&A.
   - Part 2: Technical activity called The Challenge.

- This homework is a condensed review of what you've learned in this unit. Points to consider:

   - It's critical to have a clear understanding of the concepts taught throughout this course. 
   
   - It's also important that you to have a clear understanding of "INFOSEC" terminology when interacting with other Cybersecurity professionals. Not only does this make you look professional, it also helps avoid miscommunication.
   

Some of the highlights of the things that you've learned include:

- An deep understanding of the underlying mechanics behind how web attacks are constructed from both a conceptual and practical standpoint.

- The ability to determine which mitigation strategies are most effective against various forms of web vulnerabilities.

- An understanding of how the principles of `offense informs defense` are utilized to inform security decisions by performing attacks and exploiting various web vulnerabilities from OWASP's Top 10.

The Unit 15 Homework revisits topics covered throughout the lesson. It's recommended that you re-visit the student guide and practice the activities again to strengthen your grasp on the concepts taught during the unit.


For submission, create a a file containing the answers to the questions.


### Part 1: Q&A

#### The URL Cruise Missile

The URL is the gateway to the web, providing the user with unrestricted access to all available online resources. In the wrong hands can be used as a weapon to launch attacks.

Use the graphic below to answer the following questions:

| Protocol         | Host Name                 | Path                   | Parameters               |
| ---------------- | :-----------------------: | ---------------------- | ------------------------ |
| **http://**      | **`www.buyitnow.tv`**     | **/add.asp**           | **?item=price#1999**     |


1. Which part of the URL can be manipulated by an attacker to exploit a vulnerable back-end database system? 

   `**ANS** - The parameters can be manipulated by an attacker to exploit a vulnerable back-end database.`

2. Which part of the URL can be manipulated by an attacker to cause a vulnerable web server to dump the `/etc/passwd` file? Also, name the attack used to exploit this vulnerability.

   `**ANS** - The path can be manipulated by an attacker to form what is known as the path traversal attack.`

3. Name three threat agents that can pose a risk to your organization.

   `**ANS** - Three potential threat agents are nation states, hacktivits and competitors.`


4. What kinds of sources can act as an attack vector for injection attacks?

   `**ANS** - Any type of database like SQL, Oracle, Access, etc. can be an attack vector for injection.`


5. Injection attacks exploit which part of the CIA triad?

   `**ANS** - Injection exploits can gather confidential information or alter information on a database. Therefore, injection attacks can be a part of the confidentiality and integrity parts ofthe CIa triad depending on the attack.`


6. Which two mitigation methods can be used to thwart injection attacks?

   `**ANS** - Input Validation and Input Sanitation.`

____

#### Web Server Infrastructure

Web application infrastructure includes  sub-components and external applications that provide  efficiency, scalability, reliability, robustness, and most critically, security.

- The same advancements made in web applications that provide users these conveniences are the same components that criminal hackers use to exploit them. Prudent security administrators need to be aware of how to harden such systems.


Use the graphic below to answer the following questions:

| Stage 1        | Stage 2             | Stage 3                 | Stage 4              | Stage 5          |
| :------------: | :-----------------: | :---------------------: | :------------------: | :--------------: |
| **Client**     | **Firewall**        | **Web Server**          | **Web Application**  | **Database**     |


1. What stage is the most inner part of the web architecture where data such as, customer names, addresses, account numbers, and credit card info, is stored?

   `**ANS** - Stage 5`


2. Which stage includes online forms, word processors, shopping carts, video and photo editing, spreadsheets, file scanning, file conversion, and email programs such as Gmail, Yahoo and AOL.

   `**ANS** - Stage 1`


3. What stage is the component that stores files (e.g. HTML documents, images, CSS stylesheets, and JavaScript files) that's connected to the Internet and provides support for physical data interactions between other devices connected to the web?

   `**ANS** - Stage 3`

4. What stage is where the end user interacts with the World Wide Web through the use of a web browser?

   `**ANS** - Stage 1`


5. Which stage is designed to prevent unauthorized access to and from protected web server resources?

   `**ANS** - Stage 2`

----


#### Server Side Attacks

In today’s globally connected cyber community, network and OS level attacks are well defended through the proper deployment of technical security controls such as, firewalls, IDS, Data Loss Prevention, EndPoint and security. However, web servers are accessible from anywhere on the web, making them vulnerable to attack.

1. What is the process called that cleans and scrubs user input in order to prevent it from exploiting security holes by proactively modifying user input.

   `**ANS** - Input Sanitation`


2. Name the process that tests user and application-supplied input. The process is designed to prevent malformed data from entering a data information system by verifying user input meets a specific set of criteria (i.e. a string that does not contain standalone single quotation marks).

   `**ANS** - Input Validation`


3. **Secure SDLC** is the process of ensuring security is built into web applications throughout the entire software development life cycle. Name three reasons why organization might fail at producing secure web applications.
   - Use of open-source applications for web development.
   - Absence or lack of SDLC
   - Absence or lack of Quality Assurance based Validation. 


4. How might an attacker exploit the `robots.txt` file on a web server?

   `**ANS** - An attacker can modify the file to allow them access to all files or folders.`


5. What steps can an organization take to obscure or obfuscate their contact information on domain registry web sites?

   `**ANS** - By registering for whois privacy with the domain name regsitrar.`
   
6. True or False: As a network defender, `Client-Side` validation is preferred over `Server-Side` validation because it's easier to defend against attacks.

   `**ANS** - False.`

   - Explain why you chose the answer that you did.

     `**ANS** - The end solution will likely be a combination of the two but as a web application builder, the server-side infrastructure is where the most payload and control lies. A web service provided has more control over the server-side security implementation while the client-side may be manipulated since it is part of the client's host. `

____

#### Web Application Firewalls

WAFs are designed to defend against different types of HTTP attacks and various query types such as SQLi and XSS.

WAFs are typically present on web sites that use strict transport security mechanisms such as online banking or e-commerce websites.

1. Which layer of the OSI model do WAFs operate at?

   `**ANS** - Layer7`


2. A WAF helps protect web applications by filtering and monitoring what?

   `**ANS** - Web trafffic particularly the activity going on on ports 80 and 443.`


3. True or False: A WAF based on the negative security model (Blacklisting) protects against known attacks, and a WAF based on the positive security model (Whitelisting) allows pre-approved traffic to pass.

   `**ANS** - True.`

____

#### Authentication and Access Controls

Security enhancements designed to require users to present two or more pieces of evidence or credentials when logging into an account is called multi-factor authentication.

- Legislation and regulations such as The Payment Card Industry (PCI) Data Security Standard requires the use of MFAs for all network access to a Card Data Environment (CDE).

- Security administrators should have a comprehensive understanding of the basic underlying principles of how MFA works.

1. Define all four factors of multifactor authentication and give examples of each:

   - Factor 1 - `Knowledge`

   
   - Factor 2 -  `Possession`
   
   
   - Factor 3 -  `Inherence`

   
   - Factor 4 -  `Location`

2. True or False: A password and pin is an example of 2-factor authentication.

    `**ANS** - False`
   
3. True or False: A password and `google authenticator app` is an example of 2-factor authentication.

   `**ANS** - True.`

4. What is a constrained user interface?

   `**ANS** - Restricts user access by only allowing the user to request certain functions` 

----
____

### Part 2: The Challenge 

In this activity, you will assume the role of a pen tester hired by a bank to test the security of the bank’s authentication scheme, sensitive financial data, and website interface.


#### Lab Environment   

We'll use the **Web Vulns** lab environment. To access it: 
  - Log in to the Azure Classroom Labs dashboard. 
  - Find the card with the title **Web Vulns** or **Web Vulnerability and Hardening**.
  - Click the monitor icon in the bottom-right. 
  - Select **Connect with RDP**.
  - Use Credentials (azadmin:p4ssw0rd*)

- The lab should already be started, so you should be able to connect immediately. 

- Refer to the [lab setup instructions](https://cyberxsecurity.gitlab.io/documentation/using-classroom-labs/post/2019-01-09-first-access/) for details on setting up the RDP connection.

Once the lab environment is running, open the HyperV manager and make sure that the OWASPBWA and Kali box is running.

- Then, login to the Kali VM and navigate to the IP address of the OWASPBWA machine.

- Click the option for 'WebGoat' and start the WebGoat app.

- Use the credentials: `guest`:`guest`

On the bottom of the left side of the screen, click on `Challenge` and then choose `The Challenge`.

**Note:** A common issue with this lab is the Challange activity failing to start successfully. Hit the `Restart the Lesson` button in the top right if you get an error starting the activity.

### The Challenge Instructions

#### Challenge #1

Your first mission is to break the authentication scheme. There are a number of ways to accomplish this task.

- **Hint #1**: Sometimes, form fields are shy!

- **Hint #2**: Find the hidden JavaScript.

After completing the first challenge, you will be provided with an option to continue to the next challenge.

```
Using Form Hack Firefox Extension, the username that was hidden appears to be "youaretheweakestlink"
```

![](Screenshots\Challeneg Username.png)

```
Path traversed to the java source page to find the password. Password is "goodbye". See screenshot below.
```

![](Screenshots\Challeneg Username&Password.png)

#### Challenge #2

Next, steal all of the credit card numbers from the database. 

- **Hint #1**: Sometimes cookies wear different clothes to change their appearances.

- **Hint #2**: Break your way into the conversation and inject your own ideas.

After completing the second challenge, you will be provided with an option to continue to the next challenge.

![](Screenshots\Challeneg Stage2.png)

```
After inspecting the HTTP post using BURP Suite, decided to use the password and inject an additional query. Before the query could be inserted it needed to be converted to base64 as shown in the picture below. the additions to the SQl query are essentially a wild card request that asks for everything.
```

![](Screenshots\Base64Encode.png)

```
By intercepting the post request in Burp Suite, modifying the header with the encoded SQL query and forwarding the request as shown in the picture below.
```

![](Screenshots\Challeneg Stage2 BurpSuite.png)

```
All the credit card numbers now appear on the drop down list.
```

![](Screenshots\Challeneg CreditCards.png)

#### Challenge #3

Your third and final mission is no easy feat. Your final act is to deface the website. This requires multiple skill sets, all of which you’ve learned and will need for this final act.
Two clues:

- **Hint 1**: You will need to use command injection.

- **Hint 2**: You will need to locate the `webgoat_challenge_guest.jsp` file and inject it with code in order to deface the website.

  ```
  Contrary to the hint above, the WebGoat challenge requested to deface webgoat_challenge_webgoat.jsp. The first step is to find where this file is located. By loggign in to the OWASP box and running a find command, the file was located.
  ```

  ![](Screenshots\Challeneg Stage3 webpagelocation.png)

  ```
  Using Burp Suite and intercepting the POST request, it can be identified that the File parameter resembled a command line input. The POST request was intercepted and  the File parameter was modified to append a simple HTML text in to the Web page.
  ```

  ![](Screenshots\Challeneg Stage3 Burpsuite.png)

  ```
  A picture of the defaced website is shown below
  ```

  ![](Screenshots\Challeneg Stage3 defacedwebsite.png)

  ```
  A picture of the completed challenge page is shown below
  ```

  ![](Screenshots\Challeneg CongratulationsPage.png)

![](Screenshots\CongratsChallengeComplete.png)
