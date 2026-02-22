# TodoList App

A full-stack calendar-based todo list application with React frontend and Python Flask backend.

## 📂 Project Structure

```
TODOList/
├── backend/
│   ├── app.py
│   ├── requirements.txt
│   └── .env
└── frontend/
    ├── public/
    │   ├── index.html
    │   └── 404.html (for GitHub Pages routing)
    ├── src/
    │   ├── components/
    │   │   ├── Calendar.js
    │   │   ├── TodoForm.js
    │   │   ├── TodoItem.js
    │   │   ├── TodoList.js
    │   │   └── Stats.js
    │   ├── App.js
    │   ├── index.js
    │   └── styles (CSS files)
    ├── package.json
    └── package-lock.json
```

## ✨ Features

- **Calendar View**: Interactive calendar to navigate through dates
- **Todo Management**: Create, update, and delete todos
- **Task Statistics**: View completion stats and progress
- **Responsive Design**: Works on desktop and mobile devices
- **Real-time Updates**: Live sync with backend API

## 🚀 Quick Start

### Backend Setup

```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

The backend runs on `http://localhost:5000`

### Frontend Setup

```bash
cd frontend
npm install
npm start
```

The frontend runs on `http://localhost:3000`

## 📦 Dependencies

### Backend
- Flask
- Flask-CORS
- Python-dotenv
- (See requirements.txt for full list)

### Frontend
- React 18.2.0
- React Calendar
- Axios
- Date-fns
- React Icons

## 🌐 Deployment

### GitHub Pages (Frontend)

The frontend is configured for GitHub Pages deployment:

```bash
cd frontend
npm run deploy
```

This will:
1. Build the production version
2. Deploy to GitHub Pages at: `https://sangeetha-tp-18184.github.io/TODOList`

### Backend Deployment

For backend hosting, consider:
- Heroku
- PythonAnywhere
- Railway
- AWS EC2
- DigitalOcean

## 📝 Environment Variables

### Backend (.env)
```
FLASK_ENV=development
FLASK_DEBUG=True
```

### Frontend
Update the API endpoint in `src/App.js`:
```javascript
const API_URL = process.env.REACT_APP_API_URL || 'http://localhost:5000';
```

## 🔧 API Endpoints

- `GET /api/todos` - Get all todos
- `POST /api/todos` - Create new todo
- `PUT /api/todos/<id>` - Update todo
- `DELETE /api/todos/<id>` - Delete todo

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 🛠️ Development

### Adding New Features

1. Create feature branch: `git checkout -b feature/your-feature`
2. Make changes
3. Commit: `git commit -m "Add your feature"`
4. Push: `git push origin feature/your-feature`
5. Create Pull Request

### Running Tests

```bash
npm test  # Frontend tests
pytest    # Backend tests (when configured)
```

## 📄 License

This project is open source and available under the MIT License.

## 👤 Author

sangeetha-tp-18184

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📞 Support

For issues or questions, please create an issue on GitHub.

---

**Repository**: [https://github.com/sangeetha-tp-18184/TODOList](https://github.com/sangeetha-tp-18184/TODOList)

**Live Demo**: [https://sangeetha-tp-18184.github.io/TODOList](https://sangeetha-tp-18184.github.io/TODOList)
