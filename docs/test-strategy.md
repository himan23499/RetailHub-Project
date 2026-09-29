# RetailHub Quality Engineering Test Strategy

## 1. Project Overview

RetailHub is an e-commerce application where customers can
register, authenticate, search products, manage their basket,
and complete checkout.

The objective of this project is to build a production-style
Quality Engineering framework covering UI, API, database,
security, CI/CD and AI-assisted testing.

## 2. In Scope

The following areas are included:

### UI Testing
- User registration
- Login
- Product search
- Product details
- Basket management
- Checkout
- Logout

### API Testing
- Authentication APIs
- Product APIs
- User APIs
- Basket APIs
- Checkout/order APIs

### Database Testing
- User persistence
- Product data validation
- Basket/order persistence
- Data integrity checks

### Security Testing
- Authentication
- Authorization
- Input validation
- XSS
- SQL injection awareness
- Security headers
- Session security
- OWASP ZAP baseline scanning

### Non-functional testing
- Cross-browser testing
- Basic API performance observations
- Reliability/flakiness tracking

### CI/CD
- Pull request smoke tests
- Regression tests
- Security checks
- Test reporting


## 3. Out of Scope

The following areas are outside the initial project scope:

- Real payment gateway transactions
- Real customer personal data
- Production database testing
- High-volume load testing
- Destructive security testing against public applications
- Testing third-party systems outside our control
- Mobile native application testing


## 4. User Personas

### Customer

Goal:
Purchase products successfully.

Critical activities:
- Registration
- Authentication
- Product search
- Basket management
- Checkout

### Administrator

Goal:
Manage the retail platform.

Critical activities:
- Authentication
- Product management
- User management
- Order management

### QA Engineer

Goal:
Validate product quality.

Critical activities:
- UI testing
- API testing
- Database validation
- Security testing
- CI/CD execution
- Defect analysis


## 5. Critical Business Flows

### Flow 1 — Customer Registration

User
 ↓
Open registration
 ↓
Enter valid details
 ↓
Submit
 ↓
Account created

Priority: P0

### Flow 2 — Customer Login

User
 ↓
Open login
 ↓
Enter credentials
 ↓
Authenticate
 ↓
Dashboard/home page

Priority: P0

### Flow 3 — Product Search

User
 ↓
Enter search term
 ↓
Search API
 ↓
Results displayed
 ↓
Open product

Priority: P1    

### Flow 4 — Add Product to Basket

User
 ↓
Open product
 ↓
Add to basket
 ↓
Basket updated

Priority: P0

### Flow 5 — Checkout

User
 ↓
Basket
 ↓
Enter checkout details
 ↓
Submit order
 ↓
Order confirmation

Priority: P0

### Flow 6 — Logout

User
 ↓
Logout
 ↓
Session terminated
 ↓
Protected page inaccessible

Priority: P1