<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Repositorio de Clases</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
</head>
<body class="bg-gray-900 text-white">
    <div class="flex">
        <div class="sidebar w-64 bg-gray-800 h-screen p-5">
            <div class="logo text-2xl font-bold text-center mb-10">The Hub</div>
            <ul class="nav-links">
                <li><a href="index.html" id="dashboard" class="flex items-center p-2 hover:bg-gray-700 rounded"><i class="fas fa-tachometer-alt mr-2"></i> Dashboard</a></li>
                <li><a href="https://docs.google.com/document/d/1M4xmvhHJjNSt3i-sg2_ucram2gJ44kQulcz1RqJ8K8I/edit?usp=drive_link" id="tasks" class="flex items-center p-2 hover:bg-gray-700 rounded"><i class="fas fa-tasks mr-2"></i> Tareas</a></li>
                <li><a href="https://calendar.google.com/calendar/embed?src=ee3f2903769cb310e2590eb75ecc8511de96014926bbe8ab94cd8caeb27a8a95%40group.calendar.google.com&ctz=America%2FSanto_Domingo" id="calendar" class="flex items-center p-2 hover:bg-gray-700 rounded"><i class="fas fa-calendar-alt mr-2"></i> Calendario</a></li>
                <li><a href="https://docs.google.com" id="collaboration" class="flex items-center p-2 hover:bg-gray-700 rounded"><i class="fas fa-users mr-2"></i> Colaboración</a></li>
                <li><a href="https://drive.google.com/drive/folders/1GK3reTjO4PaqhkzU-xMrDvts9FhHznCD" target="_blank" class="flex items-center p-2 hover:bg-gray-700 rounded"><i class="fas fa-folder mr-2"></i> Drive</a></li>
            </ul>
        </div>

        <div class="main-content flex-1 p-5">
            <div class="header mb-5">
                <h1 class="text-3xl font-semibold">Bienvenido The best Repository </h1>
            </div>

            <div class="search-bar flex gap-3 mb-5">
                <input type="text" placeholder="Buscar tareas..." id="searchInput" class="flex-1 p-2 rounded bg-gray-700 border border-gray-600">
                <select id="subjectFilter" class="p-2 rounded bg-gray-700 border border-gray-600">
                    <option value="">Todas las Asignaturas</option>
                    <option value="informatica">Informatica</option>
                    <option value="science">Ciencias</option>
                    <option value="history">Historia</option>
                </select>
                <select id="statusFilter" class="p-2 rounded bg-gray-700 border border-gray-600">
                    <option value="">Todos los estados</option>
                    <option value="pending">Pendiente</option>
                    <option value="progress">En progreso</option>
                    <option value="completed">Completado</option>
                </select>
            </div>

            <div class="tasks-grid grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-5">
                <!-- Las tarjetas de tareas se generarán dinámicamente -->
            </div>
        </div>
    </div>

    <button class="add-task-btn fixed bottom-5 right-5 bg-blue-600 text-white rounded-full w-12 h-12 flex items-center justify-center shadow-lg hover:bg-blue-500 transition"><i class="fas fa-plus"></i></button>

    <div class="modal fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center hidden" id="taskModal">
        <div class="modal-content bg-gray-800 p-5 rounded-lg w-11/12 max-w-md">
            <h2 class="text-xl font-semibold mb-4">Nueva Tarea</h2>
            <form id="taskForm">
                <div class="form-group mb-4">
                    <label class="block mb-1">Título</label>
                    <input type="text" name="title" required class>
                    <script src="script.js">            
                   

                    
