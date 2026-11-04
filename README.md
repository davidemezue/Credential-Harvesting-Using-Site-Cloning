# Credential Harvesting Using Site Cloning

## Overview

This lab explores credential harvesting through website cloning using the **Social-Engineer Toolkit (SET)** on Kali Linux.

Credential harvesting is a social engineering technique in which attackers use deceptive login pages to trick users into submitting sensitive information, such as usernames and passwords.

The exercise focuses on understanding how cloned login pages can receive submitted form data and why this technique presents a security risk.

## Lab Objectives

- Understand the concept of credential harvesting.
- Explore the Social-Engineer Toolkit (SET).
- Understand website cloning as a social engineering technique.
- Examine how login forms submit information through HTTP POST requests.
- Understand the risks associated with submitting credentials to deceptive websites.
- Identify security measures that help prevent credential harvesting attacks.

## Lab Environment

| Component | Details |
|---|---|
| Operating System | Kali Linux |
| Tool | Social-Engineer Toolkit (SET) |
| Lab Category | Social Engineering |
| Technique | Credential Harvesting |
| Environment | Isolated Virtual Machine |
| Target | Locally hosted mock login page |

## Tools Used

### Social-Engineer Toolkit (SET)

The Social-Engineer Toolkit is a penetration testing framework designed to support social engineering security assessments.

It provides tools for simulating different social engineering techniques, including website-based attacks.

**Launch Command:**

```bash
sudo setoolkit
```

### Network Interface Information

The local IP address of the Kali Linux virtual machine is relevant when configuring communication within an isolated lab environment.

The following command can be used to inspect network interface information:

```bash
ifconfig
```

Alternatively:

```bash
ip addr
```

## Practical Implementation

### Task 1: Starting the Social-Engineer Toolkit

The first task involved launching Kali Linux and opening a terminal.

SET was started using:

```bash
sudo setoolkit
```

This opens the SET interface, which provides access to its different social engineering assessment features.

### Task 2: Exploring Website Attack Vectors

The next stage involved exploring the website-based social engineering capabilities available in SET.

The objective was to understand the credential harvesting functionality and how deceptive login pages can be used in security assessments.

### Task 3: Understanding Credential Harvesting

Credential harvesting involves collecting information submitted through a login form.

During this exercise, the focus was on understanding how a cloned login interface can receive submitted form data.

The demonstration is restricted to a locally controlled mock login page and dummy credentials.

### Task 4: Understanding Network Configuration

The Kali Linux virtual machine's local IP address is relevant to communication between the test browser and the locally hosted demonstration environment.

Network interface information can be inspected using:

```bash
ifconfig
```

### Task 5: Understanding HTTP POST Requests

Login forms commonly use HTTP POST requests to transmit submitted form data to a server.

A POST request may contain information such as:

- Username.
- Password.
- Other login form fields.

The exercise demonstrates why credentials must only be submitted to trusted websites and why secure communication and proper website verification are important.

### Task 6: Testing With Dummy Credentials

The demonstration uses a locally controlled mock login page.

Only randomly generated test usernames and passwords should be entered.

No real accounts, third-party login pages, or personal credentials should be used.

### Task 7: Understanding Captured Form Data

The final stage focuses on understanding how form submissions can be received by a collection endpoint and why exposed credentials create a security risk.

The central security lesson is that users may unknowingly submit sensitive information to a deceptive login interface.

No real user credentials should be collected or retained.

## Key Concepts Learned

| Concept | Description |
|---|---|
| Credential Harvesting | Collecting sensitive login information through deceptive techniques. |
| Website Cloning | Reproducing a website interface, potentially for impersonation. |
| SET | A framework used for social engineering security assessments. |
| HTTP POST | An HTTP method commonly used to submit form data. |
| Social Engineering | Manipulating individuals into performing actions or disclosing information. |

## Security Relevance

Credential harvesting presents a significant security risk because compromised login information can provide unauthorized access to user accounts and organizational systems.

Security professionals should understand these techniques to identify, prevent, and respond to credential-based attacks.

### Defensive Measures

- **Website Verification:** Always verify the domain before entering login credentials.
- **Multi-Factor Authentication (MFA):** Add another authentication factor beyond passwords.
- **Phishing-Resistant Authentication:** Use FIDO2 security keys or passkeys where supported.
- **Password Managers:** Use password managers that associate credentials with legitimate website origins.
- **Security Awareness:** Educate users about deceptive login pages and phishing techniques.
- **Monitoring:** Monitor authentication logs for suspicious login attempts and unusual access patterns.

## Key Learning Outcomes

Through this lab, I explored:

1. The fundamentals of credential harvesting.
2. The role of SET in social engineering assessments.
3. How website cloning can be abused to impersonate legitimate login interfaces.
4. The purpose of HTTP POST requests in form submissions.
5. The security implications of exposing login credentials.
6. Defensive techniques for reducing the risk of credential harvesting.

## Conclusion

This lab introduced credential harvesting as a social engineering technique and explored how cloned login interfaces can be used to deceive users into submitting sensitive information.

It also highlighted the importance of website verification, secure authentication practices, phishing awareness, and defensive security controls.

Understanding how credential harvesting works is essential for cybersecurity professionals involved in penetration testing, security awareness, identity security, and incident response.

## Security Note

This exercise is intended for controlled cybersecurity education and authorized security assessments.

Use only locally controlled demonstration pages and dummy credentials. Never clone third-party login pages or collect real user credentials without explicit authorization.
