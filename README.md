<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Perfil de GitHub Único</title>
    <!-- Tailwind CSS para un diseño rápido y responsivo -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts para una tipografía única -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;700&display=swap" rel="stylesheet">
    <style>
        /* Estilos personalizados y animaciones */
        body {
            font-family: 'Space Grotesk', sans-serif;
            background-color: #10111A; /* Un fondo oscuro y moderno */
        }

        /* Animación para el gradiente del texto del encabezado */
        .animated-gradient {
            background: linear-gradient(90deg, #9333ea, #db2777, #f59e0b, #10b981);
            background-size: 400% 400%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: gradient-animation 10s ease infinite;
        }

        @keyframes gradient-animation {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        /* Efecto de borde brillante en las tarjetas */
        .card-border {
            position: relative;
            overflow: hidden;
            border-radius: 0.75rem;
            background-color: #1e293b;
        }

        .card-border::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            border-radius: 0.75rem; 
            padding: 2px;
            background: linear-gradient(90deg, #9333ea, #db2777, #f59e0b);
            -webkit-mask: 
                linear-gradient(#fff 0 0) content-box, 
                linear-gradient(#fff 0 0);
            -webkit-mask-composite: xor;
            mask-composite: exclude;
            animation: border-spin 4s linear infinite;
        }
        
        @keyframes border-spin {
            100% {
                transform: rotate(360deg);
            }
        }
    </style>
</head>
<body class="text-gray-300">

    <div class="container mx-auto max-w-4xl p-4 sm:p-6 md:p-8">
        
        <!-- Encabezado y Presentación -->
        <header class="text-center py-12">
            <h1 class="text-4xl sm:text-5xl md:text-6xl font-bold">
                ¡Hola! Soy <span class="animated-gradient">[Tu Nombre]</span>
            </h1>
            <p class="mt-4 text-lg sm:text-xl text-gray-400">Desarrollador de Software | Apasionado por la Tecnología | Creador de Soluciones</p>
        </header>

        <main class="space-y-12">
            
            <!-- Sección Sobre Mí -->
            <section id="about" class="bg-slate-800 p-8 rounded-xl shadow-lg">
                <h2 class="text-3xl font-bold text-white mb-4 border-b-2 border-purple-500 pb-2 inline-block">Sobre Mí</h2>
                <p class="text-gray-400 leading-relaxed">
                    Soy un desarrollador con experiencia en la creación de aplicaciones web modernas y eficientes. Me encanta resolver problemas complejos y aprender nuevas tecnologías. Actualmente estoy enfocado en [Tu Tecnología o Proyecto Actual]. ¡Conectemos y creemos algo increíble juntos!
                </p>
            </section>

            <!-- Tecnologías y Habilidades -->
            <section id="skills">
                <h2 class="text-3xl font-bold text-white mb-6 text-center">Mi Stack Tecnológico</h2>
                <div class="grid grid-cols-3 sm:grid-cols-4 md:grid-cols-6 gap-6 text-center">
                    <!-- Ejemplo de íconos. Puedes encontrar más en https://simpleicons.org/ -->
                    <div class="flex flex-col items-center p-4 bg-slate-800 rounded-lg hover:bg-purple-700 transition-colors duration-300">
                        <svg class="w-12 h-12" role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><title>JavaScript</title><path fill="currentColor" d="M0 0h24v24H0V0zm22.034 18.276c-.175-1.095-.82-2.145-2.005-2.82l-1.125-.63c-.96-.54-1.395-.9-1.395-1.575 0-.54.39-1.05.99-1.05.57 0 .93.39 1.05.96l1.92-.72c-.21-1.275-1.065-2.265-2.94-2.265-1.725 0-2.805 1.11-2.805 2.625 0 1.2.795 2.055 1.905 2.685l1.05.585c.87.495 1.245.81 1.245 1.5 0 .63-.495 1.14-1.125 1.14-.72 0-1.215-.495-1.35-1.14l-1.92.66c.27 1.53 1.425 2.49 3.27 2.49 1.905 0 3.09-1.11 3.09-2.7zM9.034 18.576h1.89v-7.17h-1.89v7.17zm-3.36-8.91c0-.525.435-.96.96-.96s.96.435.96.96-.435.96-.96.96-.96-.435-.96-.96zm3.36 8.91h1.89V7.416h-1.89v11.16z"/></svg>
                        <span class="mt-2 text-sm font-medium">JavaScript</span>
                    </div>
                     <div class="flex flex-col items-center p-4 bg-slate-800 rounded-lg hover:bg-pink-700 transition-colors duration-300">
                        <svg class="w-12 h-12" role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><title>React</title><path fill="currentColor" d="M12 2C6.477 2 2 6.477 2 12s4.477 10 10 10 10-4.477 10-10S17.523 2 12 2zm0 18c-4.41 0-8-3.59-8-8s3.59-8 8-8 8 3.59 8 8-3.59 8-8 8zm-1-12h2v2h-2zm0 4h2v6h-2z"/></svg>
                        <span class="mt-2 text-sm font-medium">React</span>
                    </div>
                    <div class="flex flex-col items-center p-4 bg-slate-800 rounded-lg hover:bg-yellow-600 transition-colors duration-300">
                        <svg class="w-12 h-12" role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><title>Python</title><path fill="currentColor" d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm4.29 13.88c-.68 0-1.25-.57-1.25-1.25s.57-1.25 1.25-1.25 1.25.57 1.25 1.25-.57 1.25-1.25 1.25zm-8.58 0c-.68 0-1.25-.57-1.25-1.25s.57-1.25 1.25-1.25 1.25.57 1.25 1.25-.57 1.25-1.25 1.25zM12 9.5c-.83 0-1.5-.67-1.5-1.5S11.17 6.5 12 6.5s1.5.67 1.5 1.5S12.83 9.5 12 9.5z"/></svg>
                        <span class="mt-2 text-sm font-medium">Python</span>
                    </div>
                    <div class="flex flex-col items-center p-4 bg-slate-800 rounded-lg hover:bg-green-600 transition-colors duration-300">
                        <svg class="w-12 h-12" role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><title>Node.js</title><path fill="currentColor" d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1.03 15.5l-3.48-3.48L9.66 12l-2.17-2.17 3.48-3.48L12 7.41l2.17 2.17 1.17-1.17-3.48-3.48L10.7 4 12 5.29 13.3 4l1.17 1.17-3.48 3.48L9.83 9.83l2.17 2.17L12 14.17l-2.17-2.17-1.17 1.17 3.48 3.48L13.3 18l-1.17 1.17L12 18.71l-1.03-1.04z"/></svg>
                        <span class="mt-2 text-sm font-medium">Node.js</span>
                    </div>
                     <!-- Agrega más tecnologías aquí -->
                </div>
            </section>

            <!-- Estadísticas de GitHub -->
            <!-- Para usar esto, reemplaza 'tu-usuario' con tu nombre de usuario de GitHub -->
            <section id="github-stats">
                <h2 class="text-3xl font-bold text-white mb-6 text-center">Mis Estadísticas en GitHub</h2>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                    <div class="card-border p-4">
                       <img src="https://github-readme-stats.vercel.app/api?username=tu-usuario&show_icons=true&theme=dracula&hide_border=true&include_all_commits=true&count_private=true" alt="Estadísticas de GitHub" class="w-full h-auto rounded-md" />
                    </div>
                    <div class="card-border p-4">
                        <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=tu-usuario&layout=compact&theme=dracula&hide_border=true" alt="Lenguajes más usados" class="w-full h-auto rounded-md" />
                    </div>
                </div>
            </section>

        </main>

        <!-- Pie de página y Redes Sociales -->
        <footer class="text-center py-12 mt-12">
            <h3 class="text-2xl font-bold text-white mb-4">Conecta Conmigo</h3>
            <div class="flex justify-center space-x-6">
                <a href="https://github.com/tu-usuario" target="_blank" class="text-gray-400 hover:text-purple-500 transition-colors duration-300">
                    <svg class="w-8 h-8" viewBox="0 0 24 24" fill="currentColor"><path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"/></svg>
                </a>
                <a href="https://linkedin.com/in/tu-usuario" target="_blank" class="text-gray-400 hover:text-pink-500 transition-colors duration-300">
                     <svg class="w-8 h-8" viewBox="0 0 24 24" fill="currentColor"><path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/></svg>
                </a>
                <a href="https://twitter.com/tu-usuario" target="_blank" class="text-gray-400 hover:text-yellow-500 transition-colors duration-300">
                    <svg class="w-8 h-8" viewBox="0 0 24 24" fill="currentColor"><path d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616v.064c0 2.298 1.634 4.212 3.793 4.649-.65.177-1.353.23-2.067.087.625 1.902 2.44 3.282 4.593 3.321-1.685 1.318-3.812 2.1-6.115 2.1-.398 0-.79-.023-1.175-.068 2.179 1.394 4.768 2.212 7.548 2.212 9.058 0 14.01-7.502 14.01-14.01 0-.213-.005-.426-.015-.637.961-.695 1.798-1.562 2.457-2.549z"/></svg>
                </a>
            </div>
            <p class="mt-8 text-gray-500">Diseñado con ❤️ para la comunidad de código abierto.</p>
        </footer>
    </div>

</body>
</html>
