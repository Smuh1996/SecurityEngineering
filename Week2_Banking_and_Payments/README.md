
# Tasks

### Task 1: Choose A ***or*** B
I am going to task A .

#### Task 1A: Browsers and Banking Security

Online Banking is of the most lucrative targets for phishing and scams. How do our browsers protect us against them?

Look at the following snippets from a browsers address bar:

![Bank image 1](https://github.com/ouspg/SecurityEngineering/blob/main/Week2_Banking_and_Payments/Images/bank_1.png)

![Bank image 2](https://github.com/ouspg/SecurityEngineering/blob/main/Week2_Banking_and_Payments/Images/bank_2.png)

![Bank image 3](https://github.com/ouspg/SecurityEngineering/blob/main/Week2_Banking_and_Payments/Images/bank_3.png)

**Questions:**

- What does the "Not Secure" warning mean in the first picture and what risks does visiting sites with the warning pose?

Answer: In the first picture, the word ‘Not Secure’ which appears in the address bar which means that the site address does not have HTTPS added to its URL, which encrypts data between the browser and the server. These kind of sites are rather dangerous as one can face data interception and risky for the data.

- Why does the second site show up as "trusted" to the browser?

Answer :In the second picture it appears as “trusted” whether the browser issued a valid SSL/TLS certificate. This is indication of the padlock symbol. This certificate makes sure that the information that is exchanged with the user on the site is secure.


- What other ways are there to detect a phishing/scam site? 

Answer:There are a lot of ways to detect a pishing/scam website:
Look for the existence of HTTPS and appropriate certificate.
You should also look for the website design as mostly scammers provide the low-quality site design, grammatical errors, and a lot of symbol errors.
The scamsites can also be confirmed through an official e-mail from the organization.

- Are there any tools available online?

Answer:There are a few online sites to check the phishing/scam sites.
1:Website reputation checkers like Google Safe Browsing
2:Checkphish
3:Scamvoid
4:Aura

- What is typosquatting and how does it relate to the pictures?

Answer:Typosquatting is the process of registering domains that are similar in appearance to different websites with the aim of leading the users to the wrong sites. In the pictures, similar looking URLs like "danskebankk.fi’ and "danskebank.io" are made to confuse the users.That is called typosquatting.

    - What is **UDRP** and how does it help with combatting typosquatting?
 
 Answer : UDRP stand forUniform Domain-Name Dispute-Resolution Policy (UDRP) assists the trademark proprietors legal tools with which to challenge and regain the domains that are closely similar to their trademarks.

    - If you were to own the domain **ouspg.org** and would be running your crypto banking application at **bank.ouspg.org**, what domains could you monitor for warning signs of possible phishing attempts against your customers?

Answer:If I own “ouspg.org” and run a crypto banking application at “bank.ouspg.org,” I must have an eye and monitor the domains like “ouspgg.org,” “ousgp.org,” “bankkouspg.org,” and other similar variations.To avoid Phishing Imust have a strict authentication with the similar websites.

### Task 2: Cards and Payments

**Read the following:**

https://en.wikipedia.org/wiki/Payment_card
https://en.wikipedia.org/wiki/EMV
https://en.wikipedia.org/wiki/Multi-factor_authentication

**Questions: Payments**

- Why do modern payment cards use a chip and not a magnetic stripe?

Answer:Modern payment cards contain chips because the chips are more secure than magnetic stripes. With these chips, the card produces a digital transaction code for each transaction, therefore cannot be easily fake or duplicity. On the other hand, the magnetic strip contains the static data which can be duplicated and can be legally used for fraudulent purposes.

- What are EMV Certificates and why are they relevant for payment protection?

  Answer:Basically, EMV certificates can be described as a kind of permit for credit card and payment machines. They make sure both are safe to use. This helps us to  verify that a card is real and keeps us from stealing money, making sure that the transactions safer.

- What attacks exist against payment cards?
    - Card-not-present?
    - Contactless payment?

Answer:
Card-not-present (CNP) Fraud: This kind of  happens when people shop things online without the card being there. The scammer steal card info through tricks like phishing or data breaches to make fake shopping.

Contactless Payment Attacks: Contactless payments are easy, but they can be risky. One of the example is "skimming"  when someone secretly gets your card information with a special device. In ois ther kind  "relay attack," when two devices trick the payment machine into thinking a fake card is real.

**Questions: MFA**

- How is multi-factor authentication (MFA) used in banking?

Answer:MFA in banking means you need to prove your identity in two or more ways before you can access your account. This usually combines something you know with something you have.

- How does multi-factor authentication increase payment security?

Answer:MFA makes it harder for scammers to access your account because they need more than just your password. Even if they get your password, they still need the second factor, like a code is to be sent to your phone.

- What MFA methods are you using in you daily life?

Answer:I use
Authenticator.
Fingerprint or face recognition .
Codes sent to email or phone.

- What attacks exists against different forms of 2FA?
    - Time-based-one-time-password?
    - Text Message?

Answer:
Time-Based One-Time Password
Phishing: Scammers trick you into sharing your code.
Text Message (SMS) Codes:
Someone tricks your phone company to take over your number and get your codes.

### Task 3: Card Fraud

One part of understanding payment card security is monitoring how the cards are used for frauds. The following articles are reports on card fraud by the European Central Bank and will give you an overview of how the fraud landscape has evolved between 2008-2019. Read through the articles and then answer the questions in the questions section.

**Read the following reports:**


https://www.ecb.europa.eu/pub/pdf/cardfraud/cardfraudreport201207en.pdf
https://www.ecb.europa.eu/pub/cardfraud/html/ecb.cardfraudreport202008~521edb602b.en.html
https://www.ecb.europa.eu/pub/cardfraud/html/ecb.cardfraudreport202110~cac4c418e8.en.html

**Supporting Resources:**

https://www.ecb.europa.eu/pub/pubbydate/html/index.en.html (Search: "Fraud")
https://www.ecb.europa.eu/paym/intro/mip-online/2018/html/1803_revisedpsd.en.html


**Questions:**

Write a summary (max 700 words) on "Evolution of card fraud" in which you answer **at least** the following questions:

- What kinds of card fraud exist?
- 
Answer:There are a few Card frauds come in several forms:
Card-present (CP) fraud
Card-not-present (CNP) fraud
Account takeover
Application fraud

    - How does card fraud type prevalence differ geographically?

Answer:Card fraud is different in different parts of the world. In Europe, they use  EMV chip technology that has made it much harder for criminals to duplicate the physical cards, so card-present fraud has has less chances to get in. In North America, this type of fraud has been high for a while because chip cards were made very  slowly, but things got  improved by the mid-2010s. In places like Asia and Latin America, online fraud is more common due to the boost of e-commerce and weaker security systems.

- How has the fraud landscape changed between 2008-2019? Why?
- 
Answer:Between 2008 and 2019, the fraud landscape changed significantly.When the EMV chip technology rised the Card-present fraud declined and the technology made it harder to clone physical cards.But the card-not-present (CNP) fraud like online fraud, rised due to the boost of e-commerce and online payments. As more people started shopping online and the scammers started focusing on digital transactions, which don't require any of physical cards.

    - What type of fraud has seen a notable increase during the last decade?
    - 
Anser:Card-not-present (CNP) fraud has increased over the last decade.This type of fraud, which occurs in online, phone, or mail transactions where the physical card is not required.

    - What technologies or regulations have had an impact on card fraud?

Answer:There are several technologies and regulations that have helped to reduce card fraud:
1:EMV chip technology
2:3D Secure
3:PSD2 (Payment Services Directive 2)

- How has the transaction landscape changed in the same period?

Answer:There are few things that have changed from last decade
1:Rise of e-commerce
2:Mobile payments
3:Contactless payments
These shifts made transactions more easy but also increased the risks.

    - What kind of transactions have become increasingly popular?

Answer:There are few things that have become popular
1:Online shopping
2:Mobile payments
3:Contactless payments

    - What kind of transactions have had a high risk of being fraudulent?

Answer:
1. Card-not-present (CNP) transactions  
2. High-value purchases  
3. Cross-border transactions

        - Has this changed at all during 2008-2019?
- What effect has internet and e-commerce had on card fraud?
Answer:As the internet and e-commerce are getting popular theft through cards especially card-not-present (CNP) fraud has also increased by a large percentage. Scammers have taken advantage of the digital transaction to steal and use credit and debit cards informatively.

- Why is preventing data breaches important in preventing card fraud?

Answer:Preventing data breaches important in preventing card fraud because breaches expose sensitive information making it easy for scammers to do fraud using stolen card details.Preventing breaches helps minimize financial loss for both consumers and businesses by reducing the number of fraudulent transactions

    - How does payment card tokenisation help in this?
Answer:Payment card tokenization helps prevent card fraud by  replacing sensitive card information, or the card number, as an example one can use an individual and encrypted token which these fraudsters would not recognize anyway. In case of data breach, the real card data are not disclosed so as to minimize fraud risks.

-Anything interesting you found?

---
