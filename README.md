# Portfolio Website with Direct Email Sending

A modern, responsive portfolio website with direct email functionality that sends emails server-side without opening email clients.

## Features

- ✨ Modern glassmorphism design
- 📱 Fully responsive layout
- 📧 Direct email sending (no email client required)
- 🔔 Real-time notifications
- ⚡ Fast and optimized performance

## Setup Instructions

### 1. Install Dependencies

```bash
npm install
```

### 2. Configure Email Settings

1. Copy the environment template:
   ```bash
   copy .env.example .env
   ```

2. Edit `.env` file with your Gmail credentials:
   ```
   EMAIL_USER=your-email@gmail.com
   EMAIL_PASS=your-app-password
   PORT=3000
   ```

### 3. Gmail App Password Setup

To send emails via Gmail, you need an App Password:

1. Go to [Google Account Settings](https://myaccount.google.com/)
2. Enable 2-Factor Authentication
3. Go to Security → App passwords
4. Generate a new app password for "Mail"
5. Use the 16-character password in your `.env` file

### 4. Run the Application

```bash
# Development mode (with auto-restart)
npm run dev

# Production mode
npm start
```

The website will be available at: `http://localhost:3000`

## How It Works

1. **Frontend**: Contact form collects user information
2. **Backend**: Node.js server with Express handles email sending
3. **Email Service**: Nodemailer sends emails via Gmail SMTP
4. **Notifications**: Real-time feedback shown to users

## Contact Form Features

- ✅ Form validation (all fields required)
- ✅ Email format validation
- ✅ Loading states during email sending
- ✅ Success/error notifications
- ✅ Automatic form reset on success
- ✅ Professional HTML email formatting

## Technologies Used

- **Frontend**: HTML5, CSS3, JavaScript, Tailwind CSS
- **Backend**: Node.js, Express.js
- **Email**: Nodemailer with Gmail SMTP
- **Styling**: Glassmorphism effects, animations

## File Structure

```
├── index.html          # Main portfolio page
├── server.js           # Backend server
├── package.json        # Dependencies
├── .env.example        # Environment template
├── .env               # Your email configuration (create this)
└── README.md          # This file
```

## Troubleshooting

### Email Not Sending
- Check your Gmail App Password is correct
- Ensure 2FA is enabled on your Google account
- Verify your `.env` file configuration

### Server Not Starting
- Make sure port 3000 is available
- Check if all dependencies are installed: `npm install`

### Form Not Working
- Check browser console for errors
- Ensure server is running on port 3000
- Verify network connection

## Support

If you encounter any issues, please check:
1. Console logs in browser developer tools
2. Server logs in terminal
3. Email configuration in `.env` file

---

Made with ❤️ by Sumaiya Sayyed
