## Phishing Email Investigation

## 1. What Happened??

A suspicious email was received by a user, Impersonating Paypal. Email was in German language And Was Manipulating user

## 2. Analysis Performed

File was present in "users/files/phisingemail/paypal.eml"
File was in ".eml" extension so used notepad to view backend
In notepad there was all backend of "paypal.eml" file info expect html code 
Asked to create report on give questions like :- domain url, Return path, was domain suspicious
The return path was:- "bounce@rjttznyzjjzydnillquh.designclub.uk.com"
Domain url the link from where it came was :- "https://storage.googleapis.com"
Later converted url into SHA-256 As asked to do in report 
SHA-256 :- "13945ecc33afee74ac7f72e1d5bb73050894356c4bf63d02a1a53e76830567f5"

## 3. Evidence

Suspicious return path :-
"bounce@rjttznyzjjzydnillquh.designclub.uk.com"
Suspicious Email:- 
"https://storage.googleapis.com"
Email type:- 
Phishing attemp impersonating paypal in German Language

## 4. Is it malicious??

**True Positive**

Imperonating Real brand paypal
email was suspicious 
user suspicious retuen path

## 5. Recommended Action 

User should block the sender 
Do not interact with email
should not click on any link 

## 6. Conclusion

The investigation was confirm email phishing, Impersonating Real world Brand Paypal.
