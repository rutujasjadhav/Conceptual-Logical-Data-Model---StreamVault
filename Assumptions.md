# Assumptions 

## Follow Junction Table
- This junction table resolves the many-to-many **reflexive relationship** between User Accounts.
- It allows users to follow other users within the platform.

## Subscription Table
- Three subscription tiers are defined:
  - **Basic**
  - **Premium**
  - **Family**
- Each user account is associated with **one** subscription plan.
- The subscription table is implemented as a **lookup table**.

## Generalization Translation

### Account Hierarchy
- The generalization relationship among **Account**, **User**, and **Guest** entities is implemented using `accountID` as the primary key.
- The **Account** entity serves as an abstract superclass.

### Content Hierarchy
- The same generalization approach is applied to content types.
- A single `contentID` is used to connect **Albums**, **Series**, and **Movies**.

## Viewing History
- User viewing history is tracked using the `StreamingSession` table.
- This table references the User’s `accountID` as a foreign key.

## Content Classification
- **Documentaries** are classified and stored as **Movies**.
- **Podcast series** are classified as **Albums**, with individual podcast episodes stored as **Songs**.

## File Storage
- The `file` attribute in the `Content` table stores media file references (e.g., `.mp3`, `.mp4`).
- This may be implemented as either:
  - A URL link, or
  - A file system path
- The data type is defined as **TEXT** to allow flexibility in storage approaches.

## Guest Account Limitations
Guest accounts have the following restrictions:
- Maximum streaming quality limited to **720p**
- Maximum watch time limited to **2 hours per session**

## Account Abstract Class
- The `Account` class is an **abstract class**.
- Every account instance must be either:
  - a **User** account, or
  - a **Guest** account
