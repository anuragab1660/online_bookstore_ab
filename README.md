
# Online Bookstore

An online bookstore application built with Python, CustomTkinter, and SQLite, featuring user authentication, book browsing, cart functionality, and payment integration.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Setup Instructions](#setup-instructions)
5. [Usage](#usage)
6. [Database Schema](#database-schema)
7. [Contributing](#contributing)
8. [License](#license)
9. [Contact](#contact)

## Project Overview

This project is an online bookstore application that allows users to browse books, add them to their cart, and make purchases. It includes features like user authentication, OTP-based signup, and an admin panel for managing books and orders.

## Features

- **User Authentication**: Login and signup with OTP verification.
- **Home Page**: Display books with the ability to add books via URL.
- **Search and Filter**: Search for books and filter by categories, price, etc.
- **Cart and Checkout**: Add books to the cart and proceed to checkout with a payment gateway.
- **User Profile**: Manage user profiles and view order history.
- **Admin Panel**: Manage books, users, and orders.

## Technologies Used

- **Frontend**: CustomTkinter (Python GUI library)
- **Backend**: Python, Flask
- **Database**: SQLite
- **Payment Gateway**: Stripe (or your chosen provider)
- **Other**: hashlib, smtplib (for email)

## Setup Instructions

### Prerequisites

- Python 3.x installed
- SQLite3 installed

### Installation

1. **Clone the Repository**

   \`\`\`bash
   git clone https://github.com/yourusername/online-bookstore.git
   cd online-bookstore
   \`\`\`

2. **Create a Virtual Environment**

   \`\`\`bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scriptsctivate`
   \`\`\`

3. **Install Dependencies**

   \`\`\`bash
   pip install -r requirements.txt
   \`\`\`

4. **Set Up the Database**

   \`\`\`bash
   python src/database.py
   \`\`\`

5. **Environment Variables**

   Create a `.env` file in the root directory with the following variables:

   \`\`\`env
   STRIPE_API_KEY=your_stripe_api_key
   EMAIL_ADDRESS=your_email@example.com
   EMAIL_PASSWORD=your_email_password
   \`\`\`

6. **Run the Application**

   \`\`\`bash
   python main.py
   \`\`\`

## Usage

### User Guide

1. **Login/Signup**: Use the login/signup page to authenticate. OTP verification is required for signup.
2. **Browse Books**: Browse books on the home page. Use the search bar and filters to find books.
3. **Add to Cart**: Click on books to view details and add them to the cart.
4. **Checkout**: Proceed to checkout and complete the payment process.
5. **Profile Management**: Update your profile information and view order history.
6. **Admin Panel**: Admin users can manage books, users, and orders.

### Admin Guide

1. **Login as Admin**: Admin users can log in to access the admin panel.
2. **Manage Books**: Add, edit, or delete books.
3. **Manage Users**: View and manage user accounts.
4. **Manage Orders**: View and update order statuses.

## Database Schema

- **Users**: `user_id`, `username`, `email`, `password`, `otp`
- **Books**: `book_id`, `title`, `author`, `price`, `image_url`
- **Orders**: `order_id`, `user_id`, `book_id`, `quantity`, `total_price`

## Contributing

### How to Contribute

1. **Fork the Repository**

   Click the "Fork" button at the top-right corner of this repository.

2. **Clone Your Fork**

   \`\`\`bash
   git clone https://github.com/yourusername/online-bookstore.git
   \`\`\`

3. **Create a Branch**

   \`\`\`bash
   git checkout -b feature/your-feature-name
   \`\`\`

4. **Make Changes**

   Implement your feature or bug fix.

5. **Commit and Push**

   \`\`\`bash
   git add .
   git commit -m "Add your commit message"
   git push origin feature/your-feature-name
   \`\`\`

6. **Create a Pull Request**

   Go to the original repository and create a pull request with a description of your changes.

### Code Style

- Follow PEP 8 style guidelines for Python code.
- Comment your code for better understanding.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any inquiries, please contact [Your Name](mailto:your.email@example.com).
