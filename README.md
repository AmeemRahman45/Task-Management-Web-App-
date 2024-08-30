<h1>📝 Task Manager 📝</h1>
<p>
    Welcome to the Task Manager project! This web application allows users to manage tasks efficiently with an intuitive and visually appealing interface.
</p>
<br>
<h3>🚀 Features</h3>
<ul>
    <li>📝 <strong>Task Creation</strong>: Easily add new tasks with a simple input field.</li>
    <li>✔️ <strong>Task Completion</strong>: Mark tasks as completed by clicking the complete button.</li>
    <li>🗑️ <strong>Task Deletion</strong>: Remove tasks from the list with a single click.</li>
    <li>📱 <strong>Responsive Design</strong>: Enjoy a seamless experience on both desktop and mobile devices.</li>
</ul>
<br>
<h3>🔧 Technologies Used</h3>
<ul>
    <li>HTML: Provides the structure and layout of the application.</li>
    <li>CSS: Adds stylish and responsive design, including transitions and hover effects.</li>
    <li>JavaScript: Implements functionality for task management, including adding, toggling, and deleting tasks.</li>
</ul>
<br><br>
<h3>📋 Code Explanation</h3>
<ol>
    <li>
        <h4>HTML Structure</h4>
        <pre>
&lt;!DOCTYPE html&gt;
&lt;html lang="en"&gt;
    &lt;head&gt;
        &lt;meta charset="UTF-8"&gt;
        &lt;meta name="viewport" content="width=device-width, initial-scale=1.0"&gt;
        &lt;title&gt;Stylish Task Manager&lt;/title&gt;
        &lt;link rel="stylesheet" href="/css/styles.css"&gt;
    &lt;/head&gt;
    &lt;body&gt;
        &lt;div class="container"&gt;
            &lt;h1&gt;Task Manager&lt;/h1&gt;
            &lt;div class="form-group"&gt;
                &lt;label for="taskInput"&gt;New Task&lt;/label&gt;
                &lt;input type="text" id="taskInput" placeholder="Enter task name"&gt;
            &lt;/div&gt;
            &lt;button class="btn-primary" onclick="addTask()"&gt;Add Task&lt;/button&gt;
            &lt;ul id="taskList"&gt;&lt;/ul&gt;
        &lt;/div&gt;
        &lt;script src="/js/script.js"&gt;&lt;/script&gt;
    &lt;/body&gt;
&lt;/html&gt;
        </pre>
    </li>
    <li>
        <h4>CSS Styling</h4>
        <pre>
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: 'Arial', sans-serif;
}

body {
    background: linear-gradient(135deg, #f5f7fa, #c3cfe2);
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}

.container {
    background-color: #ffffff;
    padding: 30px;
    width: 100%;
    max-width: 500px;
    border-radius: 10px;
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
}

h1 {
    font-size: 24px;
    margin-bottom: 20px;
    text-align: center;
    color: #333;
}

.form-group {
    margin-bottom: 20px;
}

label {
    display: block;
    font-size: 14px;
    color: #666;
    margin-bottom: 10px;
}

input[type="text"] {
    width: 100%;
    padding: 12px;
    border: 2px solid #ccc;
    border-radius: 5px;
    font-size: 16px;
}

.btn-primary {
    width: 100%;
    padding: 12px;
    background-color: #3498db;
    color: white;
    border: none;
    border-radius: 5px;
    font-size: 16px;
    cursor: pointer;
    margin-bottom: 20px;
}

.btn-primary:hover {
    background-color: #2980b9;
}

ul {
    list-style-type: none;
    padding: 0;
}

li {
    background-color: #f9f9f9;
    padding: 15px;
    margin-bottom: 10px;
