
# Link Me - Social Media Platform

Link Me is a social media platform similar to Instagram and Facebook, allowing users to create profiles, share posts, photos, and videos, and interact through likes, comments, and follows. It is built using PHP with PHPMyAdmin as the backend database and includes Gmail SMTP functionality for email notifications.

## Features
- **User Profiles**: Personalized profiles with bio and profile picture.
- **Post Sharing**: Share text, images, and videos.
- **Like & Comment**: Interact with posts by liking or commenting.
- **Follow System**: Follow users to get updates on their posts.
- **Notifications**: Real-time notifications for user interactions.
- **Gmail SMTP Integration**: Send email notifications (e.g., welcome emails, password reset) through Gmail's SMTP server.

## Tech Stack
- **Frontend**: HTML, CSS, JavaScript
- **Backend**: PHP
- **Database**: PHPMyAdmin (MySQL)
- **Email Service**: Gmail SMTP
- **Authentication**: PHP Sessions
- **Media Storage**: Server-based file storage for images and videos

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/link-me.git
   ```

2. **Navigate to the project directory**:
   ```bash
   cd link-me
   ```

3. **Set up the database**:
   - Open PHPMyAdmin and create a new database.
   - Import the `link_me_database.sql` file from the `database/` folder.

4. **Configure environment variables**:
   - Update `config.php` with your database credentials:
     ```php
     $dbHost = 'localhost';
     $dbUser = 'root';
     $dbPass = 'your-password';
     $dbName = 'link_me';
     ```

5. **Set up Gmail SMTP**:
   - In `config.php`, add your Gmail SMTP details:
     ```php
     $mailHost = 'smtp.gmail.com';
     $mailUsername = 'your-email@gmail.com';
     $mailPassword = 'your-app-password'; // Generate this from Gmail app passwords
     $mailPort = 587;
     $mailEncryption = 'tls';
     ```

6. **Start the PHP server**:
   - If using XAMPP or MAMP, place the project in `htdocs` and start the server.
   - Alternatively, run:
     ```bash
     php -S localhost:8000
     ```

7. **Access the application**:
   Open your browser and go to `http://localhost:8000` to start using Link Me.

## Usage
After setting up, users can sign up, create profiles, post content, follow others, and receive email notifications for certain activities (e.g., welcome emails, password recovery).

## Contributing
Feel free to contribute by submitting pull requests or opening issues. For significant changes, please open an issue first to discuss.

## License
This project is licensed under the MIT License.
