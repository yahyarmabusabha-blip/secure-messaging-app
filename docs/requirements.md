# Requirements

## 1. Problem Statement

Users need a way to communicate through the internet while keeping the content of their messages private from unauthorized access.

The goal of this project is to build a messaging system where message content is protected using end-to-end encryption.

## 2. Target Users

Users who want to communicate privately through one-to-one text messaging.

## 3. Project Goal

Build a simple one-to-one end-to-end encrypted messaging application as a Software Engineering learning project.

## 4. MVP Scope

- User registration
- User login
- User logout
- User profile
- Search users
- One-to-one conversations
- Send text messages
- Receive messages
- Real-time messaging
- Message status
- End-to-end encryption

## 5. Out of Scope

- Group chats
- Voice calls
- Video calls
- Stories
- Payments
- Channels
- File sharing
- Voice messages
- Multi-device synchronization

## 6. Functional Requirements

### FR-01
The system shall allow users to create an account.

### FR-02
The system shall allow users to log in.

### FR-03
The system shall allow users to search for other users.

### FR-04
The system shall allow users to start a one-to-one conversation.

### FR-05
The system shall allow users to send text messages.

### FR-06
The system shall allow recipients to receive messages.

### FR-07
Messages shall be encrypted before being sent to the server.

### FR-08
The recipient shall be able to decrypt received messages.

### FR-09
The system shall provide message delivery and read status.

## 7. Non-Functional Requirements

### Security
Message content should not be available to the server as plaintext.

### Performance
Messages should be delivered with low latency under normal network conditions.

### Reliability
The application should handle network failures gracefully.

### Maintainability
The codebase should follow clean architecture and separation of concerns.

### Scalability
The architecture should allow future features to be added without major restructuring.

### Usability
The application should provide a simple and understandable user interface.

## 8. User Stories

- As a user, I want to create an account so that I can use the application.
- As a user, I want to log in so that I can access my conversations.
- As a user, I want to search for another user so that I can start a conversation.
- As a user, I want to send an encrypted message so that its content remains private.
- As a recipient, I want to decrypt received messages so that I can read them.

## 9. Use Cases

### Send Message

1. User opens a conversation.
2. User writes a message.
3. User presses Send.
4. The client encrypts the message.
5. The encrypted message is sent to the server.
6. The server stores or forwards the encrypted message.
7. The recipient receives the encrypted message.
8. The recipient decrypts the message.
9. The recipient reads the message.

## 10. Security Requirements

- Do not invent cryptographic algorithms.
- Use established cryptographic protocols and trusted libraries.
- Protect private keys.
- Do not store plaintext messages on the server.
- Protect authentication credentials.
- Use secure communication between client and server.
- Clearly document the security limitations of the system.

## 11. Risks

- Incorrect encryption implementation
- Poor key management
- Authentication vulnerabilities
- Server compromise
- Database compromise
- Network attacks
- Device compromise
- Metadata leakage

## 12. Success Criteria

The MVP is considered successful when:

- Users can register.
- Users can log in.
- Users can find other users.
- Users can start conversations.
- Users can send messages.
- Recipients can receive messages.
- Messages are encrypted before leaving the client.
- The server does not receive plaintext message content.
- Recipients can decrypt and read messages.
- Basic automated tests pass.
