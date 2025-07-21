# SynerFeed

**SynerFeed** is a modern, full-stack feedback and development platform designed to foster a culture of continuous growth and recognition within organizations. Inspired by leading feedback tools, SynerFeed provides a structured and intuitive way for employees, leaders, and administrators to exchange constructive feedback, recognize contributions, and track professional development.

## Key Features (Phase 1, 2 & 3)

  * **User Management:** Comprehensive user profiles with different roles (Collaborator, Leader, Administrator) and custom fields.
  * **Structured Feedback Registration:**
      * **Types:** Categorize feedback as "Improvement," "Favorable," or "Special" (aligned with company values).
      * **Detailed Fields:** Utilize fields like Context, Behavior, Consequence, Considerations, and Combined for structured input.
      * **Value-Based Feedback:** Offer special feedback linked to company values, with supporting descriptions.
      * **Acknowledgment:** Recipients can "sign off" on received feedback.
  * **Administrative Functions:** Exclusive tools for administrators to manage users, edit/delete feedback, customize feedback fields, define company values, and update the platform's branding.
  * **Email Notifications:** Automated alerts for welcome, pending feedback acknowledgment, and password recovery.
  * **Role-Based Visibility:** Strict controls ensure users only see relevant feedback (administrators see all, leaders see their team's, collaborators see their own).
  * **Interactive Dashboards (Phase 2):** Visual metrics and rankings with data filters to track feedback activity and trends.
  * **Company News Feed / Mural (Phase 3):** A central space for company announcements, allowing posts with text, images, and files, along with like and comment functionalities.

## Architecture Overview (C4 Model)

The project architecture is documented using the C4 Model, providing different levels of detail for various stakeholders.

### System Context Diagram

This diagram shows **SynerFeed** as a central system interacting with its users (Collaborators, Leaders, Administrators) and an external Email Service.


### Container Diagram

This diagram breaks down the **SynerFeed** system into its main deployable applications and data stores: the **Web Application** (SPA), the **API** (NestJS), the **PostgreSQL Database**, and the **Redis Cache**. It illustrates how these containers interact.

### API Components Diagram

This diagram details the logical components (modules) within the **API** (NestJS), such as Authentication, Feedback, Admin, and Notification modules, and how they interact with the Data Access Layer and external services.

### Web Application Components Diagram

This diagram illustrates the key functional **modules** within the **Web Application** (SPA), including core navigation, authentication, dashboard, feedback management, and administrative modules, and their interactions with the API Integration, Global State, and Shared UI modules.