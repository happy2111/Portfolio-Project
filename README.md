# Portfolio Project

## 📖 Project Description
**Portfolio Project** is a web application that allows users to create and manage portfolios, projects, and teams. The application is designed for designers, developers, clients, and other participants who want to collaborate on projects.

---

## 🚀 Features

### 1. **Home Page**
- **Navigation**:
  - Logo.
  - Navigation menu (Portfolios, Projects, Teams, Contacts).
  - "Login" and "Sign Up" buttons.
- **Main Sections**:
  - Popular portfolios.
  - Project search with filters (category, author, rating).
  - Buttons for "Create Project" and "Find Team".
- **Footer**:
  - Contact information.
  - Social media links.
  - Legal information.

---

### 2. **User Roles**
1. **Administrator**:
   - Manage users.
   - Moderate content.
   - View statistics and reports.
2. **Portfolio Owner (Creators)**:
   - Create and edit portfolios.
   - Manage projects.
   - Join teams.
3. **Client**:
   - View portfolios.
   - Create a team or hire an existing one.
   - Leave feedback.
4. **Team Members**:
   - Participate in projects.
   - Communicate via chat.
   - Manage tasks.

---

### 3. **Project Creation**
- Users can create a project by providing:
  - Project title.
  - Description.
  - Start and end dates.
  - GitHub and deployment links.
  - Project image.
- **Error Handling**:
  - If invalid data is entered (e.g., incorrect URL), an error message is displayed to the user.

---

### 4. **Managing Project Contributors**
- Add contributors to a project:
  - Fields: name, email, GitHub and LinkedIn links, role.
  - Error handling for invalid data.
- Edit contributors:
  - Update contributor information.
  - Remove contributors from the project.

---

### 5. **Project Viewing**
- List of projects with pagination.
- Search projects by title.
- Project card:
  - Image.
  - Title.
  - End date.
- Navigate to a detailed project view page.

---

### 6. **User Profile**
- View and edit user information.
- List of projects the user is involved in.
- Manage portfolios.

---

### 7. **Additional Features**
- **Chat**:
  - Communication between team members.
- **Task Management**:
  - Assign tasks to team members.
  - Track task statuses.
- **User Rating**:
  - Evaluate each team member's contribution to the project.

---

## 🛠️ Installation and Setup

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/Portfolio-Project.git
cd Portfolio-Project
```

### 2. Install Dependencies
Make sure Node.js is installed. Then run:
```bash
npm install
```

### 3. Run the Project
To start the project in development mode:
```bash
npm run dev
```

To build the project:
```bash
npm run build
```

---

## 📂 Project Structure

```
Portfolio-Project/
├── public/                # Static files
├── src/
│   ├── assets/            # Images and icons
│   ├── components/        # Reusable components
│   ├── pages/             # Application pages
│   │   ├── Home.jsx       # Home page
│   │   ├── Projects.jsx   # Projects page
│   │   ├── Profile.jsx    # Profile page
│   │   └── ProjectCreate.jsx # Project creation page
│   ├── styles/            # Application styles
│   └── App.jsx            # Main application component
├── package.json           # Project dependencies
├── vite.config.js         # Vite configuration
└── README.md              # Documentation
```

---

## 📋 API

### 1. **Create a Project**
**URL**: `POST /projects/`  
**Sample Data**:
```json
{
  "title": "My Project",
  "description": "This is a test project",
  "start_time": "2025-05-01",
  "end_time": "2025-05-31",
  "git_hub": "https://github.com/example",
  "deploy_link": "https://example.com"
}
```

### 2. **Add a Contributor**
**URL**: `POST /project-contributors/`  
**Sample Data**:
```json
{
  "full_name": "John Doe",
  "email": "john.doe@example.com",
  "github_link": "https://github.com/johndoe",
  "linkedin_link": "https://linkedin.com/in/johndoe",
  "position": "Developer"
}
```

---

## 🧑‍💻 Developers
- **Frontend**: Me
- **Backend**: Shohruh

---

If you have ideas for improvements, feel free to create an **Issue** or submit a **Pull Request**. Thank you for using our project! 😊
