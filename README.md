<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RTC Robotics Club</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
</head>
<body class="bg-gray-100 text-gray-900 font-sans">
    <!-- Navigation Bar -->
    <nav class="bg-blue-700 text-white py-4">
        <div class="container mx-auto flex justify-between items-center">
            <h1 class="text-2xl font-bold">RTC Robotics Club</h1>
            <div class="space-x-4">
                <a href="#calendar" class="hover:underline">Calendar</a>
                <a href="#projects" class="hover:underline">Projects</a>
                <a href="#contact" class="hover:underline">Contact</a>
                <a href="#completed-projects" class="hover:underline">Completed Projects</a>
            </div>
        </div>
    </nav>

    <!-- Calendar Section -->
    <section id="calendar" class="container mx-auto my-10 p-6 bg-white shadow rounded-lg">
        <h2 class="text-3xl font-bold mb-4">Meeting Calendar</h2>
        <div class="flex items-center justify-between mb-4">
            <button id="weekView" class="px-4 py-2 bg-blue-600 text-white rounded hover:bg-blue-500">Week View</button>
            <button id="monthView" class="px-4 py-2 bg-blue-600 text-white rounded hover:bg-blue-500">Month View</button>
        </div>
        <div id="calendarDisplay" class="p-4">
            <!-- Calendar will be displayed here -->
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="container mx-auto my-10 p-6 bg-white shadow rounded-lg">
        <h2 class="text-3xl font-bold mb-4">Current & Proposed Projects</h2>
        <ul class="space-y-3">
            <li class="p-4 bg-gray-100 rounded">Project 1: Autonomous Drone</li>
            <li class="p-4 bg-gray-100 rounded">Project 2: Robotic Arm</li>
            <li class="p-4 bg-gray-100 rounded">Project 3: Machine Learning Rover</li>
            <!-- Add more projects as needed -->
        </ul>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="container mx-auto my-10 p-6 bg-white shadow rounded-lg">
        <h2 class="text-3xl font-bold mb-4">Contact Information</h2>
        <ul class="space-y-3">
            <li class="p-4 bg-gray-100 rounded">John Doe - Lead Engineer - johndoe@example.com</li>
            <li class="p-4 bg-gray-100 rounded">Jane Smith - Mechanical Engineer - janesmith@example.com</li>
            <li class="p-4 bg-gray-100 rounded">...other members...</li>
        </ul>
    </section>

    <!-- Completed Projects Section -->
    <section id="completed-projects" class="container mx-auto my-10 p-6 bg-white shadow rounded-lg">
        <h2 class="text-3xl font-bold mb-4">Completed Projects</h2>
        <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4">
            <div class="p-4 bg-gray-100 rounded">Completed Project 1: Robotic Arm</div>
            <div class="p-4 bg-gray-100 rounded">Completed Project 2: Smart Cart</div>
            <div class="p-4 bg-gray-100 rounded">Completed Project 3: Vision-Guided Rover</div>
            <!-- Additional completed projects as needed -->
        </div>
    </section>

    <!-- JavaScript for Calendar Functionality -->
    <script>
        // Initialize the calendar
        document.getElementById('weekView').onclick = () => {
            document.getElementById('calendarDisplay').innerHTML = '<p>Week view: Meetings every Wednesday at 5 PM</p>';
        };
        document.getElementById('monthView').onclick = () => {
            document.getElementById('calendarDisplay').innerHTML = '<p>Month view: Meetings on 1st, 2nd, and last Wednesday of each month at 5 PM</p>';
        };
    </script>
</body>
</html>
