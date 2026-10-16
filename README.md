<!DOCTYPE html>
<html lang="fr" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>E-Portfolio | Étudiant Ingénieur ENSEEIHT</title>
    
    <!-- Fonts: Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <!-- Icons: FontAwesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        navy: {
                            800: '#1e3a8a',
                            900: '#172554',
                        },
                        accent: {
                            500: '#0ea5e9', // Sky blue
                            600: '#0284c7',
                        }
                    }
                }
            }
        }
    </script>
    <style>
        /* Custom styles for elements that need extra finesse */
        body { font-family: 'Inter', sans-serif; }
        .glass-nav {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid rgba(0,0,0,0.05);
        }
        .section-padding { padding-top: 6rem; padding-bottom: 6rem; }
        .card-hover {
            transition: all 0.3s ease;
        }
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1), 0 8px 10px -6px rgba(0, 0, 0, 0.1);
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 antialiased selection:bg-accent-500 selection:text-white">

    <!-- Navigation -->
    <nav class="fixed w-full z-50 glass-nav transition-all duration-300" id="navbar">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-16 items-center">
                <!-- Logo / Name -->
                <div class="flex-shrink-0 flex items-center cursor-pointer" onclick="window.scrollTo(0,0)">
                    <span class="font-bold text-xl tracking-tight text-navy-900">E-Portfolio<span class="text-accent-500">.</span></span>
                </div>
                
                <!-- Desktop Menu -->
                <div class="hidden md:flex space-x-8">
                    <a href="#welcome" class="text-sm font-medium text-slate-600 hover:text-accent-600 transition-colors">Accueil</a>
                    <a href="#projects" class="text-sm font-medium text-slate-600 hover:text-accent-600 transition-colors">Projets</a>
                    <a href="#career" class="text-sm font-medium text-slate-600 hover:text-accent-600 transition-colors">Carrière</a>
                    <a href="#mobility" class="text-sm font-medium text-slate-600 hover:text-accent-600 transition-colors">Mobilité</a>
                    <a href="#passions" class="text-sm font-medium text-slate-600 hover:text-accent-600 transition-colors">Passions</a>
                    <a href="#civic" class="text-sm font-medium text-slate-600 hover:text-accent-600 transition-colors">Engagement Civique</a>
                </div>

                <!-- Mobile Menu Button -->
                <div class="md:hidden flex items-center">
                    <button id="mobile-menu-btn" class="text-slate-600 hover:text-navy-900 focus:outline-none">
                        <i class="fa-solid fa-bars text-2xl"></i>
                    </button>
                </div>
            </div>
        </div>

        <!-- Mobile Menu Panel -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t border-slate-100 shadow-lg absolute w-full">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#welcome" class="block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:bg-slate-50 hover:text-accent-600">Accueil</a>
                <a href="#projects" class="block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:bg-slate-50 hover:text-accent-600">Projets</a>
                <a href="#career" class="block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:bg-slate-50 hover:text-accent-600">Carrière</a>
                <a href="#mobility" class="block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:bg-slate-50 hover:text-accent-600">Mobilité</a>
                <a href="#passions" class="block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:bg-slate-50 hover:text-accent-600">Passions</a>
                <a href="#civic" class="block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:bg-slate-50 hover:text-accent-600">Engagement Civique</a>
            </div>
        </div>
    </nav>

    <!-- 1. Welcome Section -->
    <section id="welcome" class="relative pt-32 pb-20 lg:pt-48 lg:pb-32 bg-navy-900 overflow-hidden">
        <!-- Background decorative elements -->
        <div class="absolute inset-0 opacity-10">
            <svg class="absolute left-0 bottom-0 h-full w-full" preserveAspectRatio="none" viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M0 100C40 0 60 0 100 100Z" fill="#ffffff" />
            </svg>
        </div>
        
        <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center lg:text-left flex flex-col lg:flex-row items-center">
            <div class="lg:w-2/3 pr-0 lg:pr-12">
                <span class="text-accent-500 font-semibold tracking-wider uppercase text-sm mb-4 block">Génie Électrique & Management</span>
                <h1 class="text-4xl sm:text-5xl md:text-6xl font-bold text-white mb-6 leading-tight">
                    Construire l'avenir de <br/>
                    <span class="text-transparent bg-clip-text bg-gradient-to-r from-accent-500 to-teal-400">l'énergie et l'industrie.</span>
                </h1>
                <p class="text-lg md:text-xl text-slate-300 mb-10 max-w-2xl mx-auto lg:mx-0 leading-relaxed border-l-4 border-accent-500 pl-4">
                    "Bienvenue sur mon e-portfolio. Je suis étudiant ingénieur en 3EA (Électronique, Énergie Électrique et Automatique) à l'ENSEEIHT, en alternance chez Enedis en tant qu'Appui au management."
                </p>
                <div class="flex flex-col sm:flex-row justify-center lg:justify-start space-y-4 sm:space-y-0 sm:space-x-4">
                    <a href="#projects" class="bg-accent-600 hover:bg-accent-500 text-white font-medium py-3 px-8 rounded-full transition-colors shadow-lg hover:shadow-accent-500/30 text-center">
                        Voir mes projets
                    </a>
                    <a href="#career" class="bg-white/10 hover:bg-white/20 text-white border border-white/20 font-medium py-3 px-8 rounded-full transition-colors text-center backdrop-blur-sm">
                        Mon profil professionnel
                    </a>
                </div>
            </div>
            
            <div class="lg:w-1/3 mt-12 lg:mt-0 relative hidden md:block">
                <!-- Profile Image Placeholder -->
                <div class="relative w-64 h-64 mx-auto lg:w-80 lg:h-80">
                    <div class="absolute inset-0 bg-gradient-to-tr from-accent-500 to-navy-800 rounded-full animate-pulse opacity-20 blur-xl"></div>
                    <img src="https://placehold.co/400x400/1e3a8a/ffffff?text=Photo+Profil" alt="Portrait" class="relative w-full h-full object-cover rounded-full border-4 border-white/10 shadow-2xl z-10">
                    
                    <!-- Badges -->
                    <div class="absolute -bottom-4 -left-4 bg-white p-3 rounded-xl shadow-xl z-20 flex items-center space-x-2">
                        <img src="https://placehold.co/40x40/0ea5e9/ffffff?text=N7" alt="ENSEEIHT" class="w-8 h-8 rounded-md">
                        <span class="text-xs font-bold text-slate-800">ENSEEIHT</span>
                    </div>
                    <div class="absolute top-8 -right-8 bg-white p-3 rounded-xl shadow-xl z-20 flex items-center space-x-2">
                        <img src="https://placehold.co/40x40/10b981/ffffff?text=EN" alt="Enedis" class="w-8 h-8 rounded-md">
                        <span class="text-xs font-bold text-slate-800">Enedis</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 2. Projects Section -->
    <section id="projects" class="section-padding bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-navy-900 mb-4">Projets & Réalisations</h2>
                <div class="h-1 w-20 bg-accent-500 mx-auto rounded"></div>
                <p class="mt-6 text-slate-600">Découvrez une sélection de mes projets académiques à l'ENSEEIHT et de mes missions en entreprise chez Enedis, structurés selon la méthode Class 4.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <!-- Project Card 1 (Company) -->
                <div class="bg-slate-50 rounded-2xl p-8 border border-slate-100 card-hover">
                    <div class="flex items-center justify-between mb-4">
                        <span class="text-xs font-semibold px-3 py-1 bg-green-100 text-green-700 rounded-full uppercase tracking-wide">Entreprise (Enedis)</span>
                        <i class="fa-solid fa-bolt text-slate-300 text-xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-navy-900 mb-6">Titre du projet d'entreprise (Appui Management)</h3>
                    
                    <div class="space-y-4">
                        <div>
                            <h4 class="text-sm font-bold text-slate-800 uppercase flex items-center"><i class="fa-solid fa-bullseye text-accent-500 mr-2"></i> Problem (Contexte)</h4>
                            <p class="text-sm text-slate-600 mt-1">[Décrivez ici la problématique, le besoin de l'entreprise ou le contexte du réseau électrique]</p>
                        </div>
                        <div>
                            <h4 class="text-sm font-bold text-slate-800 uppercase flex items-center"><i class="fa-solid fa-user-gear text-accent-500 mr-2"></i> Role (Mon rôle)</h4>
                            <p class="text-sm text-slate-600 mt-1">[Décrivez vos responsabilités en tant qu'appui au management]</p>
                        </div>
                        <div>
                            <h4 class="text-sm font-bold text-slate-800 uppercase flex items-center"><i class="fa-solid fa-screwdriver-wrench text-accent-500 mr-2"></i> Methods (Méthodes)</h4>
                            <p class="text-sm text-slate-600 mt-1">[Outils de gestion, méthodes Lean, logiciels spécifiques, indicateurs de performance utilisés]</p>
                        </div>
                        <div>
                            <h4 class="text-sm font-bold text-slate-800 uppercase flex items-center"><i class="fa-solid fa-chart-line text-accent-500 mr-2"></i> Outcomes (Résultats)</h4>
                            <p class="text-sm text-slate-600 mt-1">[Qu'avez-vous produit ? Livrables, améliorations des processus, metrics atteints]</p>
                        </div>
                        <div class="bg-blue-50 p-3 rounded-lg border border-blue-100">
                            <h4 class="text-sm font-bold text-navy-900 uppercase flex items-center"><i class="fa-solid fa-lightbulb text-yellow-500 mr-2"></i> Lessons (Leçons apprises)</h4>
                            <p class="text-sm text-slate-700 mt-1">[Compétences managériales développées, gestion du changement, etc.]</p>
                        </div>
                    </div>
                </div>

                <!-- Project Card 2 (Academic) -->
                <div class="bg-slate-50 rounded-2xl p-8 border border-slate-100 card-hover">
                    <div class="flex items-center justify-between mb-4">
                        <span class="text-xs font-semibold px-3 py-1 bg-blue-100 text-blue-700 rounded-full uppercase tracking-wide">Académique (ENSEEIHT)</span>
                        <i class="fa-solid fa-microchip text-slate-300 text-xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-navy-900 mb-6">Titre du projet 3EA (Électronique / Énergie)</h3>
                    
                    <div class="space-y-4">
                        <div>
                            <h4 class="text-sm font-bold text-slate-800 uppercase flex items-center"><i class="fa-solid fa-bullseye text-accent-500 mr-2"></i> Problem (Problème)</h4>
                            <p class="text-sm text-slate-600 mt-1">[Définition du système technique à concevoir, simuler ou optimiser]</p>
                        </div>
                        <div>
                            <h4 class="text-sm font-bold text-slate-800 uppercase flex items-center"><i class="fa-solid fa-users text-accent-500 mr-2"></i> Role (Mon rôle)</h4>
                            <p class="text-sm text-slate-600 mt-1">[Travail en équipe, rôle spécifique (chef de projet, concepteur...)]</p>
                        </div>
                        <div>
                            <h4 class="text-sm font-bold text-slate-800 uppercase flex items-center"><i class="fa-solid fa-code text-accent-500 mr-2"></i> Methods (Méthodes)</h4>
                            <p class="text-sm text-slate-600 mt-1">[Outils (Matlab, Simulink, Altium, C/C++), théorèmes et approches techniques]</p>
                        </div>
                        <div>
                            <h4 class="text-sm font-bold text-slate-800 uppercase flex items-center"><i class="fa-solid fa-check-circle text-accent-500 mr-2"></i> Outcomes (Résultats)</h4>
                            <p class="text-sm text-slate-600 mt-1">[Maquette fonctionnelle, rapport d'étude, soutenance, code validé]</p>
                        </div>
                        <div class="bg-blue-50 p-3 rounded-lg border border-blue-100">
                            <h4 class="text-sm font-bold text-navy-900 uppercase flex items-center"><i class="fa-solid fa-lightbulb text-yellow-500 mr-2"></i> Lessons (Leçons apprises)</h4>
                            <p class="text-sm text-slate-700 mt-1">[Compétences techniques acquises, gestion du temps, résolution de problèmes]</p>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-10">
                <button class="text-accent-600 font-medium hover:text-navy-900 transition-colors inline-flex items-center">
                    <i class="fa-solid fa-plus-circle mr-2"></i> Ajouter de futurs projets
                </button>
            </div>
        </div>
    </section>

    <!-- 3. Career Section -->
    <section id="career" class="section-padding bg-slate-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-navy-900 mb-4">Carrière & Objectifs</h2>
                <div class="h-1 w-20 bg-accent-500 mx-auto rounded"></div>
                <p class="mt-6 text-slate-600">Préparation à mon insertion professionnelle : candidatures ciblées, profil LinkedIn optimisé et réseau.</p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-3 gap-8">
                <!-- Column 1: Applications -->
                <div class="lg:col-span-2 space-y-6">
                    <div class="bg-white p-8 rounded-2xl shadow-sm border border-slate-100 h-full">
                        <div class="flex items-center mb-6">
                            <div class="w-12 h-12 rounded-full bg-navy-100 flex items-center justify-center text-navy-900 mr-4">
                                <i class="fa-solid fa-file-contract text-xl"></i>
                            </div>
                            <h3 class="text-2xl font-bold text-navy-900">Candidature Cible</h3>
                        </div>
                        
                        <div class="mb-6 pb-6 border-b border-slate-100">
                            <h4 class="font-semibold text-slate-800 mb-2">1. Offre d'emploi (Job Ad)</h4>
                            <p class="text-sm text-slate-600 mb-3">Poste visé (ex: Ingénieur d'Affaires, Ingénieur Smart Grids) à l'international ou en France.</p>
                            <div class="bg-slate-50 p-4 rounded-lg border border-dashed border-slate-300 text-center">
                                <span class="text-slate-400 text-sm italic">[Capture d'écran ou lien vers l'offre d'emploi réelle]</span>
                            </div>
                        </div>

                        <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                            <div class="bg-blue-50/50 p-5 rounded-xl border border-blue-100 hover:border-accent-300 transition-colors cursor-pointer group">
                                <i class="fa-solid fa-file-pdf text-3xl text-red-500 mb-3 group-hover:scale-110 transition-transform"></i>
                                <h4 class="font-bold text-slate-800">Mon CV (English)</h4>
                                <p class="text-xs text-slate-500 mt-1">CV adapté à l'offre ciblée, incluant mon alternance.</p>
                                <a href="#" class="text-accent-600 text-sm font-medium mt-3 inline-block">Voir le document &rarr;</a>
                            </div>
                            
                            <div class="bg-blue-50/50 p-5 rounded-xl border border-blue-100 hover:border-accent-300 transition-colors cursor-pointer group">
                                <i class="fa-solid fa-envelope-open-text text-3xl text-accent-500 mb-3 group-hover:scale-110 transition-transform"></i>
                                <h4 class="font-bold text-slate-800">Cover Letter</h4>
                                <p class="text-xs text-slate-500 mt-1">Lettre de motivation en anglais répondant point par point à l'annonce.</p>
                                <a href="#" class="text-accent-600 text-sm font-medium mt-3 inline-block">Voir le document &rarr;</a>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Column 2: Network & Interviews -->
                <div class="space-y-6">
                    <!-- LinkedIn -->
                    <div class="bg-white p-6 rounded-2xl shadow-sm border border-slate-100">
                        <div class="flex items-center justify-between mb-4">
                            <h3 class="text-lg font-bold text-navy-900">Réseau Professionnel</h3>
                            <i class="fa-brands fa-linkedin text-blue-600 text-2xl"></i>
                        </div>
                        <p class="text-sm text-slate-600 mb-4">Mon profil LinkedIn est à jour, mettant en valeur ma formation ENSEEIHT et mon alternance actuelle chez Enedis.</p>
                        <a href="https://linkedin.com/" target="_blank" class="w-full block text-center bg-blue-600 hover:bg-blue-700 text-white font-medium py-2 px-4 rounded-lg transition-colors">
                            Visiter mon profil LinkedIn
                        </a>
                    </div>

                    <!-- My Job Glasses -->
                    <div class="bg-white p-6 rounded-2xl shadow-sm border border-slate-100">
                        <h3 class="text-lg font-bold text-navy-900 mb-4 flex items-center">
                            <i class="fa-solid fa-glasses mr-2 text-accent-500"></i> Entretiens Réseau
                        </h3>
                        <p class="text-xs text-slate-500 mb-4 italic">Deux entretiens My Job Glasses (qui, pourquoi, leçons apprises).</p>
                        
                        <div class="space-y-4">
                            <div class="border-l-2 border-accent-500 pl-3">
                                <h4 class="text-sm font-bold text-slate-800">[Nom du contact 1]</h4>
                                <p class="text-xs text-slate-600">Rôle & Entreprise</p>
                                <p class="text-xs text-slate-500 mt-1"><strong>Ce que j'ai appris :</strong> [Bref résumé de l'échange et des conseils obtenus]</p>
                            </div>
                            <div class="border-l-2 border-accent-500 pl-3">
                                <h4 class="text-sm font-bold text-slate-800">[Nom du contact 2]</h4>
                                <p class="text-xs text-slate-600">Rôle & Entreprise</p>
                                <p class="text-xs text-slate-500 mt-1"><strong>Ce que j'ai appris :</strong> [Bref résumé de l'échange et des conseils obtenus]</p>
                            </div>
                        </div>
                    </div>

                    <!-- Elevator Pitch -->
                    <div class="bg-navy-900 text-white p-6 rounded-2xl shadow-lg relative overflow-hidden">
                        <div class="absolute top-0 right-0 p-4 opacity-20">
                            <i class="fa-solid fa-video text-6xl"></i>
                        </div>
                        <h3 class="text-lg font-bold mb-2 relative z-10">Elevator Pitch</h3>
                        <p class="text-xs text-slate-300 mb-4 relative z-10">Vidéo de 3 min (anglais) : présent, passé (bref), futur.</p>
                        <button class="bg-white text-navy-900 text-sm font-bold py-2 px-4 rounded-lg w-full hover:bg-accent-50 transition-colors relative z-10 flex justify-center items-center">
                            <i class="fa-solid fa-play-circle mr-2"></i> Lancer la vidéo
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 4. Mobility Section -->
    <section id="mobility" class="section-padding bg-white border-t border-slate-100">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col md:flex-row items-start md:items-center justify-between mb-12">
                <div class="max-w-2xl">
                    <h2 class="text-3xl font-bold text-navy-900 mb-2">Projet de Mobilité Internationale</h2>
                    <div class="h-1 w-16 bg-accent-500 rounded mb-4"></div>
                    <p class="text-slate-600">Exploration de destinations pour valider l'expérience internationale requise, en accord avec mon alternance chez Enedis.</p>
                </div>
                <div class="mt-6 md:mt-0 opacity-20 hidden md:block">
                    <i class="fa-solid fa-earth-europe text-8xl text-navy-900"></i>
                </div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <!-- Destination 1 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-sm border border-slate-100 card-hover">
                    <div class="h-32 bg-slate-200 relative">
                        <img src="https://placehold.co/600x300/1e293b/ffffff?text=Destination+1" alt="Destination" class="w-full h-full object-cover">
                        <div class="absolute top-3 right-3 bg-white px-2 py-1 rounded text-xs font-bold text-navy-900 shadow">Choix 1</div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-slate-800 mb-2">[Pays / Ville / Université]</h3>
                        <p class="text-sm font-semibold text-accent-600 mb-3">Motivations :</p>
                        <p class="text-sm text-slate-600 mb-4">[Pourquoi cette destination ? Culture, excellence académique dans le domaine de l'énergie/électronique...]</p>
                        
                        <div class="bg-slate-50 p-3 rounded border border-slate-200">
                            <p class="text-xs font-semibold text-slate-700"><i class="fa-solid fa-briefcase text-slate-400 mr-1"></i> Faisabilité Enedis :</p>
                            <p class="text-xs text-slate-500 mt-1">[Modalités de détachement, accord de l'entreprise, période ciblée]</p>
                        </div>
                    </div>
                </div>

                <!-- Destination 2 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-sm border border-slate-100 card-hover">
                    <div class="h-32 bg-slate-200 relative">
                        <img src="https://placehold.co/600x300/334155/ffffff?text=Destination+2" alt="Destination" class="w-full h-full object-cover">
                        <div class="absolute top-3 right-3 bg-white px-2 py-1 rounded text-xs font-bold text-navy-900 shadow">Choix 2</div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-slate-800 mb-2">[Pays / Ville / Université]</h3>
                        <p class="text-sm font-semibold text-accent-600 mb-3">Motivations :</p>
                        <p class="text-sm text-slate-600 mb-4">[Découverte d'un nouveau marché de l'énergie, apprentissage d'une langue...]</p>
                        
                        <div class="bg-slate-50 p-3 rounded border border-slate-200">
                            <p class="text-xs font-semibold text-slate-700"><i class="fa-solid fa-briefcase text-slate-400 mr-1"></i> Faisabilité Enedis :</p>
                            <p class="text-xs text-slate-500 mt-1">[Modalités pratiques et logistiques]</p>
                        </div>
                    </div>
                </div>

                <!-- Destination 3 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-sm border border-slate-100 card-hover">
                    <div class="h-32 bg-slate-200 relative">
                        <img src="https://placehold.co/600x300/475569/ffffff?text=Destination+3" alt="Destination" class="w-full h-full object-cover">
                        <div class="absolute top-3 right-3 bg-white px-2 py-1 rounded text-xs font-bold text-navy-900 shadow">Choix 3</div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-slate-800 mb-2">[Pays / Ville / Université]</h3>
                        <p class="text-sm font-semibold text-accent-600 mb-3">Motivations :</p>
                        <p class="text-sm text-slate-600 mb-4">[Réseau de partenaires ENSEEIHT, attrait personnel...]</p>
                        
                        <div class="bg-slate-50 p-3 rounded border border-slate-200">
                            <p class="text-xs font-semibold text-slate-700"><i class="fa-solid fa-briefcase text-slate-400 mr-1"></i> Faisabilité Enedis :</p>
                            <p class="text-xs text-slate-500 mt-1">[Plan de secours ou option alternative]</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 5. Passions Section -->
    <section id="passions" class="section-padding bg-slate-900 text-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Passions & Centres d'intérêt</h2>
                <div class="h-1 w-20 bg-accent-500 mx-auto rounded"></div>
                <p class="mt-6 text-slate-300">Ce qui m'anime au-delà des études et du travail : sport, arts, vie associative et projets personnels.</p>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6">
                <!-- Sport -->
                <div class="bg-slate-800/50 backdrop-blur border border-slate-700 p-6 rounded-2xl text-center hover:bg-slate-800 transition-colors">
                    <div class="w-16 h-16 bg-slate-700 rounded-full flex items-center justify-center mx-auto mb-4 text-accent-400 text-2xl">
                        <i class="fa-solid fa-person-running"></i>
                    </div>
                    <h3 class="text-lg font-bold mb-2">Sport</h3>
                    <p class="text-sm text-slate-400">[Ex: Pratique du marathon, esprit d'équipe au rugby, dépassement de soi]</p>
                </div>

                <!-- Arts -->
                <div class="bg-slate-800/50 backdrop-blur border border-slate-700 p-6 rounded-2xl text-center hover:bg-slate-800 transition-colors">
                    <div class="w-16 h-16 bg-slate-700 rounded-full flex items-center justify-center mx-auto mb-4 text-pink-400 text-2xl">
                        <i class="fa-solid fa-palette"></i>
                    </div>
                    <h3 class="text-lg font-bold mb-2">Arts & Culture</h3>
                    <p class="text-sm text-slate-400">[Ex: Photographie, musique, créativité appliquée à la résolution de problèmes]</p>
                </div>

                <!-- Associations -->
                <div class="bg-slate-800/50 backdrop-blur border border-slate-700 p-6 rounded-2xl text-center hover:bg-slate-800 transition-colors">
                    <div class="w-16 h-16 bg-slate-700 rounded-full flex items-center justify-center mx-auto mb-4 text-yellow-400 text-2xl">
                        <i class="fa-solid fa-users"></i>
                    </div>
                    <h3 class="text-lg font-bold mb-2">Vie Associative</h3>
                    <p class="text-sm text-slate-400">[Ex: Membre du BDE, club robotique N7, organisation d'événements]</p>
                </div>

                <!-- Personal Projects -->
                <div class="bg-slate-800/50 backdrop-blur border border-slate-700 p-6 rounded-2xl text-center hover:bg-slate-800 transition-colors">
                    <div class="w-16 h-16 bg-slate-700 rounded-full flex items-center justify-center mx-auto mb-4 text-green-400 text-2xl">
                        <i class="fa-solid fa-rocket"></i>
                    </div>
                    <h3 class="text-lg font-bold mb-2">Projets Persos</h3>
                    <p class="text-sm text-slate-400">[Ex: Impression 3D, domotique, programmation Arduino à domicile]</p>
                </div>
            </div>
        </div>
    </section>

    <!-- 6. Civic Engagement Section -->
    <section id="civic" class="section-padding bg-slate-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="bg-white rounded-3xl shadow-lg border border-slate-100 overflow-hidden flex flex-col md:flex-row">
                <div class="md:w-2/5 bg-accent-600 p-10 text-white flex flex-col justify-center">
                    <i class="fa-solid fa-hand-holding-heart text-5xl mb-6 opacity-80"></i>
                    <h2 class="text-3xl font-bold mb-4">Engagement Civique (RSE)</h2>
                    <p class="text-accent-100 mb-8">Investissement sociétal et validation des heures d'engagement obligatoires du cursus ingénieur.</p>
                    
                    <!-- Progress Bar -->
                    <div class="bg-navy-900/30 rounded-lg p-5">
                        <div class="flex justify-between text-sm font-semibold mb-2">
                            <span>Progression RSE</span>
                            <span>[XX] / [Total] Heures</span>
                        </div>
                        <div class="w-full bg-white/20 rounded-full h-2.5">
                            <div class="bg-white h-2.5 rounded-full" style="width: 45%"></div>
                        </div>
                    </div>
                </div>
                
                <div class="md:w-3/5 p-10 lg:p-12">
                    <h3 class="text-xl font-bold text-navy-900 mb-6 border-b border-slate-100 pb-4">Actions réalisées ou planifiées</h3>
                    
                    <div class="space-y-6">
                        <!-- Action 1 -->
                        <div class="flex">
                            <div class="flex-shrink-0 mt-1">
                                <div class="w-8 h-8 rounded-full bg-green-100 flex items-center justify-center border border-green-200">
                                    <i class="fa-solid fa-check text-green-600 text-xs"></i>
                                </div>
                            </div>
                            <div class="ml-4">
                                <h4 class="text-base font-bold text-slate-800">[Titre de l'action terminée]</h4>
                                <p class="text-xs text-accent-600 font-semibold mb-1">[Date] • [Nombre] heures</p>
                                <p class="text-sm text-slate-600">Description détaillée de la mission (ex: Tutorat, aide alimentaire, sensibilisation écologique). Impact personnel et apport à la communauté.</p>
                            </div>
                        </div>
                        
                        <!-- Action 2 -->
                        <div class="flex">
                            <div class="flex-shrink-0 mt-1">
                                <div class="w-8 h-8 rounded-full bg-slate-100 flex items-center justify-center border border-slate-200">
                                    <i class="fa-solid fa-hourglass-half text-slate-500 text-xs"></i>
                                </div>
                            </div>
                            <div class="ml-4">
                                <h4 class="text-base font-bold text-slate-800">[Titre de l'action planifiée]</h4>
                                <p class="text-xs text-slate-500 font-semibold mb-1">Prévu pour [Mois/Année] • [Nombre] heures estimées</p>
                                <p class="text-sm text-slate-600">Description du projet futur. Organisme d'accueil visé (Croix-Rouge, Secours Populaire, associations étudiantes solidaires).</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-navy-900 pt-12 pb-8 border-t border-navy-800 text-slate-400">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="text-xl font-bold text-white tracking-tight mb-4">E-Portfolio<span class="text-accent-500">.</span></h2>
            <p class="text-sm mb-6 max-w-md mx-auto">Préparé dans le cadre du module "Marketing 4 Careers" - ENSEEIHT - Alternance Enedis.</p>
            <div class="flex justify-center space-x-6 mb-8">
                <a href="#" class="text-slate-400 hover:text-white transition-colors">
                    <span class="sr-only">LinkedIn</span>
                    <i class="fa-brands fa-linkedin text-xl"></i>
                </a>
                <a href="#" class="text-slate-400 hover:text-white transition-colors">
                    <span class="sr-only">GitHub</span>
                    <i class="fa-brands fa-github text-xl"></i>
                </a>
                <a href="mailto:#" class="text-slate-400 hover:text-white transition-colors">
                    <span class="sr-only">Email</span>
                    <i class="fa-solid fa-envelope text-xl"></i>
                </a>
            </div>
            <p class="text-xs border-t border-navy-800 pt-8">
                &copy; 2026 Étudiant ENSEEIHT 3EA. Tous droits réservés.
            </p>
        </div>
    </footer>

    <!-- Scripts -->
    <script>
        // Mobile Menu Toggle
        const btn = document.getElementById('mobile-menu-btn');
        const menu = document.getElementById('mobile-menu');

        btn.addEventListener('click', () => {
            menu.classList.toggle('hidden');
        });

        // Close mobile menu when a link is clicked
        const mobileLinks = menu.querySelectorAll('a');
        mobileLinks.forEach(link => {
            link.addEventListener('click', () => {
                menu.classList.add('hidden');
            });
        });

        // Navbar styling on scroll
        const navbar = document.getElementById('navbar');
        window.addEventListener('scroll', () => {
            if (window.scrollY > 20) {
                navbar.classList.add('shadow-md');
                navbar.classList.add('py-0');
                navbar.classList.remove('py-2');
            } else {
                navbar.classList.remove('shadow-md');
                navbar.classList.add('py-2');
                navbar.classList.remove('py-0');
            }
        });
        
        // Initial setup for navbar padding
        if (window.scrollY <= 20) {
            navbar.classList.add('py-2');
        }
    </script>
</body>
</html>
