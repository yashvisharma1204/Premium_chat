# Premium Chat
A modern, real-time chat application with sleek dark UI, private spaces, and seamless collaboration features.

## Features ✨

- **Real-time messaging** with Socket.IO
- **Private chat spaces** with member management
- **Glossy UI** with modern design
- **User authentication** (login/signup)
- **Responsive design** works on all devices
- **Message history** for each space

## Technologies Used 🛠️

### Frontend
- HTML5, CSS3 (with modern Flexbox/Grid layouts)
- JavaScript (ES6+)
- [Socket.IO](https://socket.io/) for real-time communication
- [Font Awesome](https://fontawesome.com/) for icons

### Backend
- Python with Flask
- MongoDB for data storage
- JWT for authentication

## Installation & Setup ⚙️

### Prerequisites
- Python 3.8+
- MongoDB Atlas account or local MongoDB instance

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/premium-chat.git
   cd premium-chat
   ```

2. Set up virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up environment variables:
   Create a `.env` file in the root directory:
   ```
   MONGO_URI=your_mongodb_connection_string
   ```

5. Run the application:
   ```bash
   python app.py
   ```

6. Access the app at:
   ```
   http://localhost:5000
   ```

## Project Structure 📂

```
premium-chat/
├── static/
│   ├── styles.css       # Main stylesheet
│   └── ...              # Other static assets
├── templates/
│   ├── index.html       # Homepage/dashboard
│   ├── view_room.html   # Chat room interface
│   ├── create_room.html # Space creation form
│   ├── login.html       # Login page
│   ├── signup.html      # Signup page
│   └── ...              # Other templates
├── app.py               # Flask application
├── db.py                # Database functions
├── user.py              # User functions
├── requirements.txt     # Python dependencies
└── README.md            # This file
```

## API Endpoints 🌐

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/rooms` | GET | Get all rooms for current user |
| `/api/rooms` | POST | Create new room |
| `/api/rooms/<room_id>` | GET | Get room details |
| `/api/rooms/<room_id>/messages` | GET | Get room message history |
| `/api/rooms/<room_id>/members` | GET | Get room members |

## Socket.IO Events 📡

| Event | Direction | Description |
|-------|-----------|-------------|
| `join_room` | Client → Server | Join a chat room |
| `leave_room` | Client → Server | Leave a chat room |
| `send_message` | Client → Server | Send new message |
| `receive_message` | Server → Client | Receive new message |


## Screenshots 📸

### Dashboard
![Screenshot 2025-04-09 184608](https://github.com/user-attachments/assets/c268626c-6f29-4232-86ab-bfcf8e239b2e)


### Chat Room
![Screenshot 2025-04-22 220213](https://github.com/user-attachments/assets/65034f09-5ec9-48b4-a3e7-9ad16c980bf6)


### Create Space
![Screenshot 2025-04-13 172112](https://github.com/user-attachments/assets/38702d5f-0b12-4dec-b0dc-7bc48ac52576)


## Contributing 🤝

Contributions are welcome! Please follow these steps:

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License 📄

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
