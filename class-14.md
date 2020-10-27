# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-13) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-15)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

1. When is Basic Authorization used vs. Bearer Authorization?

2. What does the JSON Web Token package do?
provide all the methods needed for generating (sign) and verifying JWTs (verify).

3. What considerations should we make when creating and storing a SECRET?
making sure that it is kept in a safe place and only available for authorised members.

## Term

encryption: encoding information from normal(readable) text to a ciphertext.
token: a secure format used to send information between two parties
bearer: the owner of the token
secret: a confidential key used for encoding the data inside a token
JSON Web Token: Is an open standard that will help protect information sent between ant two users, where the information is digitally signed therefore trusted and secured.

## RBAC (Role Base Access Control)

Assigning system access to users based on their roles in the organization (estricting system access to authorized users.).

### advanntages

* easier to audit user rights, and to correct any issues identified.
* easy to implement, and will make the ongoing management of access rights much easier and more secure.

### RBAC implementation

1. Figure out what resources you have for which you need to control access
2. group your workforce members into roles with common access needs
3. figure out which role(s) each employee belongs in, and set their access accordingly.
4. Never make one-off changes
5. Audit