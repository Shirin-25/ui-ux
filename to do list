<!DOCTYPE html>
<html>
<head>
    <title>To-Do List</title>

    
</head>

<body>

    <h1>To-Do List</h1>

    <input type="text" id="taskInput" placeholder="Enter a task">
    <button onclick="addTask()">Add</button>

    <ul id="taskList"></ul>

    <script>

        function addTask() {

            let input = document.getElementById("taskInput");
            let task = input.value;

            if (task === "") {
                alert("Please enter a task");
                return;
            }

            let li = document.createElement("li");

            li.innerHTML = `
                <span>${task}</span>
                <button onclick="editTask(this)">Edit</button>
                <button onclick="deleteTask(this)">Delete</button>
            `;

            document.getElementById("taskList").appendChild(li);

            input.value = "";
        }

        function editTask(button) {

            let li = button.parentElement;
            let span = li.querySelector("span");

            let newTask = prompt("Edit your task:", span.innerText);

            if (newTask !== null && newTask !== "") {
                span.innerText = newTask;
            }
        }

        function deleteTask(button) {

            let li = button.parentElement;

            li.remove();
        }

    </script>

</body>
</html>
