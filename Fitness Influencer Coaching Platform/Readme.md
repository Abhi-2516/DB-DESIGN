# 🏋️ Online Fitness Coaching Platform – ER Diagram

## 📌 Problem Statement

A fitness influencer starts an online coaching business by training clients through Instagram DMs and video calls. As the business grows, they need a structured system to manage:

* Clients and trainers
* Coaching plans and subscriptions
* Sessions and consultations
* Client progress tracking (weight, measurements, reports)
* Payments and subscriptions

The platform should support different types of users:

* Some clients only book consultations
* Some purchase long-term coaching plans
* Some attend live sessions, while others follow routines independently

---

## 🎯 Objective

To design a normalized and scalable ER diagram that supports:

* Trainer–client relationships
* Plan and subscription management
* Session scheduling
* Progress tracking and check-ins
* Payment handling

---

## 🧠 My Approach

In my approach, I first identified the core entities such as Trainer, Client, Plan, and Subscription.

* I used a Subscription entity to track which client purchased which plan, along with start and end dates.
* I separated Sessions (live/consultation interactions) from Check-ins (weekly updates) because they serve different purposes.
* I created a Progress entity to store fitness data like weight, body fat, and measurements without mixing it with user data.
* I linked Payments to subscriptions to maintain transaction history.
* I ensured proper use of Primary Keys and Foreign Keys to maintain relationships and data integrity.

Overall, the design focuses on:

* Real-world usability
* Clean separation of concerns
* Scalability for future growth

---

## 🔗 Key Relationships

* One Trainer can handle multiple Clients (via sessions)
* One Client can have multiple Subscriptions
* One Plan can be subscribed to by many clients
* One Client can attend multiple Sessions
* One Client can submit multiple Check-ins
* One Client can have multiple Progress records
* Each Subscription can have associated Payments

---

## 🧩 Core Features Modeled

* User Management (Trainer & Client)
* Coaching Plans & Subscriptions
* Sessions & Consultations
* Progress Tracking
* Check-ins & Feedback
* Payment Management

---

## 🖼️ ER Diagram

![ER Diagram](db.png)


---

## 🚀 How to Use

* Open the diagram image to view:

  * Entities and attributes
  * Primary Keys (PK)
  * Foreign Keys (FK)
  * Relationships and structure

---

## 📚 Tools Used

* Draw.io (for ER diagram design)
* GitHub (for hosting and submission)

---

## ✅ Conclusion

This ER design models a real-world online fitness coaching platform by clearly separating plans, sessions, and progress tracking. It ensures a scalable and maintainable system that can support both small-scale coaching and future platform growth.
