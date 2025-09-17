# Prog6212-PoePart1
https://github.com/OmphileMolatlhegi/Prog6212-PoePart1.git
Overview
The Contract Monthly Claim System (CMCS) is a .NET web-based application designed to streamline the process of submitting and approving monthly claims for Independent Contractor (IC) lecturers. This system serves as a crucial tool for managing the complex process of claim submissions, verifications, and approvals within academic institutions.

Features
Current Prototype Features

Dashboard: Overview of claim statistics, recent activity, and quick actions
Submit Claims: Form for creating new monthly claims with itemized billing
My Claims: View and manage all submitted claims with filtering capabilities
Document Management: Interface for uploading supporting documents (in development)
Reports: Analytics and reporting functionality (in development)
User Management: System for managing user roles and permissions (in development)
System Settings: Configuration options for the application (in development)

User Roles
Lecturers: Can submit claims, upload documents, and track claim status
Programme Coordinators: Can verify and approve claims
Academic Managers: Can provide final approval on claims
Technology Stack
Frontend: HTML5, CSS3, JavaScript, Bootstrap 5, Font Awesome
Backend: ASP.NET Core MVC (to be implemented)
Database: SQL Server (to be implemented)
Version Control: Git with GitHub
Database Design
Tables
Users: Stores information about all system users

Claims: Central table storing all claim information
ClaimItems: Stores individual line items within a claim
Documents: Manages supporting documents uploaded for claims
Approvals: Tracks approval history for audit purposes

Relationships
Users → Claims: One-to-Many
Claims → ClaimItems: One-to-Many
Claims → Documents: One-to-Many
Claims → Approvals: One-to-Many
Usage Guide
For Lecturers
Log in to the system
Navigate to "Submit New Claim" to create a monthly claim
Add line items with hours worked and rates

Upload supporting documents
Submit the claim for approval
Track claim status in "My Claims" section
For Programme Coordinators
Log in to the system
Review claims awaiting approval in the dashboard

Verify claim details and supporting documents
Approve or reject claims with comments
For Academic Managers
Log in to the system

Review claims approved by Programme Coordinators
Provide final approval or rejection
Monitor overall claim statistics and trends
Development Status
Completed
Project structure setup

MVC architecture implementation
Responsive UI design
Dashboard layout
Navigation system
Claim submission form UI
Claims listing page

In Progress
Database integration
User authentication
Claim processing logic

Document upload functionality
Reporting system
Future Enhancements
Email notifications
Advanced reporting
Bulk operations
API integration
Mobile application
Contributing
Fork the repository

Create a feature branch (git checkout -b feature/AmazingFeature)
Commit your changes (git commit -m 'Add some AmazingFeature')
Push to the branch (git push origin feature/AmazingFeature)
Open a Pull Request

Version Control
Commit Message Convention
feat: New feature implementation

fix: Bug fix
docs: Documentation changes
style: Code formatting changes
refactor: Code refactoring
test: Adding or updating tests
chore: Maintenance tasks

Branch Strategy
main: Production-ready code
develop: Integration branch for features
feature/*: New feature development
hotfix/*: Critical bug fixes

API Documentation (Future Implementation)
Endpoints
GET /api/claims: Retrieve all claims
POST /api/claims: Create a new claim
GET /api/claims/{id}: Retrieve a specific claim
PUT /api/claims/{id}: Update a claim
DELETE /api/claims/{id}: Delete a claim
POST /api/claims/{id}/approve: Approve a claim
POST /api/claims/{id}/reject: Reject a claim

Testing
Test Cases (To Be Implemented)
User authentication and authorization
Claim submission and validation
Approval workflow testing
Document upload and retrieval
Report generation

Testing Tools
xUnit for unit testing
Moq for mocking dependencies
Selenium for UI testing
Postman for API testing

Deployment
Development Environment
IIS Express for local development
SQL Server LocalDB for database

Production Environment
Azure App Service for hosting
Azure SQL Database for data storage
Azure Blob Storage for document storage
