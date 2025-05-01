<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Instituto Café - Tecnologia com Sabor</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f8f9fa;
        }
        
        .hero-gradient {
            background: linear-gradient(135deg, #6f42c1 0%, #d63384 100%);
        }
        
        .product-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        
        .nav-link:hover {
            color: #d63384 !important;
        }
        
        .coffee-icon {
            animation: float 3s ease-in-out infinite;
        }
        
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }
        
        .deal-timer {
            background: linear-gradient(45deg, #ff6b6b, #f06595);
        }
    </style>
</head>
<body>
    <!-- Top Bar -->
    <div class="bg-gray-900 text-white py-2 px-4 text-sm">
        <div class="container mx-auto flex justify-between items-center">
            <div class="flex space-x-4">
                <span><i class="fas fa-phone-alt mr-1"></i> (11) 4002-8922</span>
                <span><i class="fas fa-envelope mr-1"></i> contato@institutocafe.com.br</span>
            </div>
            <div class="flex space-x-4">
                <a href="#" class="hover:text-purple-300"><i class="fab fa-facebook-f"></i></a>
                <a href="#" class="hover:text-purple-300"><i class="fab fa-instagram"></i></a>
                <a href="#" class="hover:text-purple-300"><i class="fab fa-twitter"></i></a>
                <a href="#" class="hover:text-purple-300"><i class="fab fa-youtube"></i></a>
            </div>
        </div>
    </div>

    <!-- Header -->
    <header class="bg-white shadow-sm sticky top-0 z-50">
        <div class="container mx-auto px-4 py-4">
            <div class="flex items-center justify-between">
                <!-- Logo -->
                <div class="flex items-center space-x-2">
                    <div class="coffee-icon text-3xl text-purple-600">
                        <i class="fas fa-coffee"></i>
                    </div>
                    <h1 class="text-2xl font-bold text-gray-800">
                        <span class="text-purple-600">Instituto</span> <span class="text-gray-700">Café</span>
                    </h1>
                </div>
                
                <!-- Search -->
                <div class="hidden md:flex flex-1 mx-8">
                    <div class="relative w-full">
                        <input type="text" placeholder="Buscar produtos..." class="w-full px-4 py-2 border border-gray-300 rounded-l-lg focus:outline-none focus:ring-2 focus:ring-purple-500">
                        <button class="bg-purple-600 text-white px-4 py-2 rounded-r-lg hover:bg-purple-700 transition">
                            <i class="fas fa-search"></i>
                        </button>
                    </div>
                </div>
                
                <!-- User Menu -->
                <div class="flex items-center space-x-4">
                    <a href="#" class="text-gray-700 hover:text-purple-600">
                        <i class="fas fa-user text-xl"></i>
                    </a>
                    <a href="#" class="text-gray-700 hover:text-purple-600 relative">
                        <i class="fas fa-heart text-xl"></i>
                        <span class="absolute -top-2 -right-2 bg-purple-600 text-white text-xs rounded-full h-5 w-5 flex items-center justify-center">3</span>
                    </a>
                    <a href="#" class="text-gray-700 hover:text-purple-600 relative">
                        <i class="fas fa-shopping-cart text-xl"></i>
                        <span class="absolute -top-2 -right-2 bg-purple-600 text-white text-xs rounded-full h-5 w-5 flex items-center justify-center">5</span>
                    </a>
                </div>
            </div>
        </div>
    </header>

    <!-- Navigation -->
    <nav class="bg-purple-700 text-white">
        <div class="container mx-auto px-4">
            <div class="flex items-center justify-between py-3">
                <div class="flex items-center space-x-1">
                    <button class="bg-purple-800 px-4 py-2 rounded-md flex items-center">
                        <i class="fas fa-bars mr-2"></i>
                        <span>Categorias</span>
                    </button>
                </div>
                
                <div class="hidden md:flex space-x-6">
                    <a href="#" class="nav-link hover:text-purple-200 font-medium">Home</a>
                    <a href="#" class="nav-link hover:text-purple-200 font-medium">Promoções</a>
                    <a href="#" class="nav-link hover:text-purple-200 font-medium">Hardware</a>
                    <a href="#" class="nav-link hover:text-purple-200 font-medium">Periféricos</a>
                    <a href="#" class="nav-link hover:text-purple-200 font-medium">Notebooks</a>
                    <a href="#" class="nav-link hover:text-purple-200 font-medium">Smartphones</a>
                </div>
                
                <div class="flex items-center space-x-2">
                    <span class="text-sm">Atendimento</span>
                    <i class="fas fa-headset"></i>
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero-gradient text-white py-12">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-8 md:mb-0">
                    <h2 class="text-4xl font-bold mb-4">Tecnologia com Sabor</h2>
                    <p class="text-xl mb-6">Os melhores produtos de tecnologia com a qualidade que só o Instituto Café oferece.</p>
                    <div class="flex space-x-4">
                        <button class="bg-white text-purple-700 px-6 py-3 rounded-lg font-bold hover:bg-gray-100 transition">Comprar Agora</button>
                        <button class="border-2 border-white px-6 py-3 rounded-lg font-bold hover:bg-white hover:text-purple-700 transition">Saiba Mais</button>
                    </div>
                </div>
                <div class="md:w-1/2 flex justify-center">
                    <img src="https://images.unsplash.com/photo-1518770660439-4636190af475?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Tecnologia e Café" class="rounded-lg shadow-xl w-full max-w-md">
                </div>
            </div>
        </div>
    </section>

    <!-- Categories -->
    <section class="py-8 bg-white">
        <div class="container mx-auto px-4">
            <h3 class="text-2xl font-bold mb-6 text-gray-800">Categorias em Destaque</h3>
            <div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-6 gap-4">
                <a href="#" class="bg-gray-100 p-4 rounded-lg text-center hover:bg-purple-100 transition">
                    <div class="text-purple-600 text-3xl mb-2">
                        <i class="fas fa-laptop"></i>
                    </div>
                    <span class="font-medium">Notebooks</span>
                </a>
                <a href="#" class="bg-gray-100 p-4 rounded-lg text-center hover:bg-purple-100 transition">
                    <div class="text-purple-600 text-3xl mb-2">
                        <i class="fas fa-mobile-alt"></i>
                    </div>
                    <span class="font-medium">Smartphones</span>
                </a>
                <a href="#" class="bg-gray-100 p-4 rounded-lg text-center hover:bg-purple-100 transition">
                    <div class="text-purple-600 text-3xl mb-2">
                        <i class="fas fa-headphones"></i>
                    </div>
                    <span class="font-medium">Áudio</span>
                </a>
                <a href="#" class="bg-gray-100 p-4 rounded-lg text-center hover:bg-purple-100 transition">
                    <div class="text-purple-600 text-3xl mb-2">
                        <i class="fas fa-gamepad"></i>
                    </div>
                    <span class="font-medium">Games</span>
                </a>
                <a href="#" class="bg-gray-100 p-4 rounded-lg text-center hover:bg-purple-100 transition">
                    <div class="text-purple-600 text-3xl mb-2">
                        <i class="fas fa-desktop"></i>
                    </div>
                    <span class="font-medium">Monitores</span>
                </a>
                <a href="#" class="bg-gray-100 p-4 rounded-lg text-center hover:bg-purple-100 transition">
                    <div class="text-purple-600 text-3xl mb-2">
                        <i class="fas fa-microchip"></i>
                    </div>
                    <span class="font-medium">Hardware</span>
                </a>
            </div>
        </div>
    </section>

    <!-- Flash Deal -->
    <section class="py-8 bg-gray-100">
        <div class="container mx-auto px-4">
            <div class="flex items-center justify-between mb-6">
                <h3 class="text-2xl font-bold text-gray-800">Oferta Relâmpago</h3>
                <div class="deal-timer text-white px-4 py-2 rounded-lg font-bold">
                    <i class="fas fa-bolt mr-2"></i>
                    <span id="countdown">23:59:59</span>
                </div>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <!-- Deal Product 1 -->
                <div class="bg-white rounded-lg overflow-hidden shadow-md product-card transition duration-300">
                    <div class="relative">
                        <img src="https://images.unsplash.com/photo-1593642632823-8f785ba67e45?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1632&q=80" alt="Notebook Gamer" class="w-full h-48 object-cover">
                        <div class="absolute top-2 left-2 bg-red-600 text-white px-2 py-1 rounded text-xs font-bold">-25%</div>
                    </div>
                    <div class="p-4">
                        <h4 class="font-bold text-lg mb-2">Notebook Gamer Avançado</h4>
                        <div class="flex items-center mb-2">
                            <div class="text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star-half-alt"></i>
                            </div>
                            <span class="text-gray-600 text-sm ml-2">(128)</span>
                        </div>
                        <div class="mb-2">
                            <span class="text-gray-500 line-through text-sm">R$ 6.999,00</span>
                            <span class="text-red-600 font-bold ml-2">R$ 5.249,00</span>
                        </div>
                        <div class="text-green-600 text-sm font-medium mb-3">
                            <i class="fas fa-check-circle"></i> Em estoque
                        </div>
                        <button class="w-full bg-purple-600 text-white py-2 rounded-lg hover:bg-purple-700 transition">
                            <i class="fas fa-cart-plus mr-2"></i> Comprar
                        </button>
                    </div>
                </div>
                
                <!-- Deal Product 2 -->
                <div class="bg-white rounded-lg overflow-hidden shadow-md product-card transition duration-300">
                    <div class="relative">
                        <img src="https://images.unsplash.com/photo-1592899677977-9c10ca588bbd?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1632&q=80" alt="Smartphone" class="w-full h-48 object-cover">
                        <div class="absolute top-2 left-2 bg-red-600 text-white px-2 py-1 rounded text-xs font-bold">-15%</div>
                    </div>
                    <div class="p-4">
                        <h4 class="font-bold text-lg mb-2">Smartphone Premium</h4>
                        <div class="flex items-center mb-2">
                            <div class="text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                            <span class="text-gray-600 text-sm ml-2">(256)</span>
                        </div>
                        <div class="mb-2">
                            <span class="text-gray-500 line-through text-sm">R$ 4.599,00</span>
                            <span class="text-red-600 font-bold ml-2">R$ 3.909,15</span>
                        </div>
                        <div class="text-green-600 text-sm font-medium mb-3">
                            <i class="fas fa-check-circle"></i> Em estoque
                        </div>
                        <button class="w-full bg-purple-600 text-white py-2 rounded-lg hover:bg-purple-700 transition">
                            <i class="fas fa-cart-plus mr-2"></i> Comprar
                        </button>
                    </div>
                </div>
                
                <!-- Deal Product 3 -->
                <div class="bg-white rounded-lg overflow-hidden shadow-md product-card transition duration-300">
                    <div class="relative">
                        <img src="https://images.unsplash.com/photo-1590658268037-6bf12165a8df?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1632&q=80" alt="Fone de Ouvido" class="w-full h-48 object-cover">
                        <div class="absolute top-2 left-2 bg-red-600 text-white px-2 py-1 rounded text-xs font-bold">-30%</div>
                    </div>
                    <div class="p-4">
                        <h4 class="font-bold text-lg mb-2">Fone Bluetooth Elite</h4>
                        <div class="flex items-center mb-2">
                            <div class="text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="far fa-star"></i>
                            </div>
                            <span class="text-gray-600 text-sm ml-2">(87)</span>
                        </div>
                        <div class="mb-2">
                            <span class="text-gray-500 line-through text-sm">R$ 899,00</span>
                            <span class="text-red-600 font-bold ml-2">R$ 629,30</span>
                        </div>
                        <div class="text-green-600 text-sm font-medium mb-3">
                            <i class="fas fa-check-circle"></i> Em estoque
                        </div>
                        <button class="w-full bg-purple-600 text-white py-2 rounded-lg hover:bg-purple-700 transition">
                            <i class="fas fa-cart-plus mr-2"></i> Comprar
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Featured Products -->
    <section class="py-8 bg-white">
        <div class="container mx-auto px-4">
            <h3 class="text-2xl font-bold mb-6 text-gray-800">Destaques</h3>
            
            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">
                <!-- Product 1 -->
                <div class="bg-white rounded-lg overflow-hidden shadow-md product-card transition duration-300 border border-gray-200">
                    <div class="relative">
                        <img src="https://images.unsplash.com/photo-1544244011-7e4b40315b7b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Monitor Gamer" class="w-full h-48 object-cover">
                    </div>
                    <div class="p-4">
                        <h4 class="font-bold text-lg mb-2">Monitor Gamer 27" 144Hz</h4>
                        <div class="flex items-center mb-2">
                            <div class="text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star-half-alt"></i>
                            </div>
                            <span class="text-gray-600 text-sm ml-2">(92)</span>
                        </div>
                        <div class="mb-2">
                            <span class="text-purple-600 font-bold">R$ 1.899,00</span>
                        </div>
                        <div class="text-green-600 text-sm font-medium mb-3">
                            <i class="fas fa-check-circle"></i> Em estoque
                        </div>
                        <button class="w-full bg-purple-600 text-white py-2 rounded-lg hover:bg-purple-700 transition">
                            <i class="fas fa-cart-plus mr-2"></i> Comprar
                        </button>
                    </div>
                </div>
                
                <!-- Product 2 -->
                <div class="bg-white rounded-lg overflow-hidden shadow-md product-card transition duration-300 border border-gray-200">
                    <div class="relative">
                        <img src="https://images.unsplash.com/photo-1587829741301-dc798b83add3?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1365&q=80" alt="Teclado Mecânico" class="w-full h-48 object-cover">
                    </div>
                    <div class="p-4">
                        <h4 class="font-bold text-lg mb-2">Teclado Mecânico RGB</h4>
                        <div class="flex items-center mb-2">
                            <div class="text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="far fa-star"></i>
                            </div>
                            <span class="text-gray-600 text-sm ml-2">(64)</span>
                        </div>
                        <div class="mb-2">
                            <span class="text-purple-600 font-bold">R$ 459,90</span>
                        </div>
                        <div class="text-green-600 text-sm font-medium mb-3">
                            <i class="fas fa-check-circle"></i> Em estoque
                        </div>
                        <button class="w-full bg-purple-600 text-white py-2 rounded-lg hover:bg-purple-700 transition">
                            <i class="fas fa-cart-plus mr-2"></i> Comprar
                        </button>
                    </div>
                </div>
                
                <!-- Product 3 -->
                <div class="bg-white rounded-lg overflow-hidden shadow-md product-card transition duration-300 border border-gray-200">
                    <div class="relative">
                        <img src="https://images.unsplash.com/photo-1527814050087-3793815479db?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1528&q=80" alt="Mouse Gamer" class="w-full h-48 object-cover">
                    </div>
                    <div class="p-4">
                        <h4 class="font-bold text-lg mb-2">Mouse Gamer 16000DPI</h4>
                        <div class="flex items-center mb-2">
                            <div class="text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                            <span class="text-gray-600 text-sm ml-2">(143)</span>
                        </div>
                        <div class="mb-2">
                            <span class="text-purple-600 font-bold">R$ 289,90</span>
                        </div>
                        <div class="text-green-600 text-sm font-medium mb-3">
                            <i class="fas fa-check-circle"></i> Em estoque
                        </div>
                        <button class="w-full bg-purple-600 text-white py-2 rounded-lg hover:bg-purple-700 transition">
                            <i class="fas fa-cart-plus mr-2"></i> Comprar
                        </button>
                    </div>
                </div>
                
                <!-- Product 4 -->
                <div class="bg-white rounded-lg overflow-hidden shadow-md product-card transition duration-300 border border-gray-200">
                    <div class="relative">
                        <img src="https://images.unsplash.com/photo-1591488320449-011701bb6704?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="SSD 1TB" class="w-full h-48 object-cover">
                    </div>
                    <div class="p-4">
                        <h4 class="font-bold text-lg mb-2">SSD NVMe 1TB</h4>
                        <div class="flex items-center mb-2">
                            <div class="text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                            <span class="text-gray-600 text-sm ml-2">(201)</span>
                        </div>
                        <div class="mb-2">
                            <span class="text-purple-600 font-bold">R$ 499,90</span>
                        </div>
                        <div class="text-green-600 text-sm font-medium mb-3">
                            <i class="fas fa-check-circle"></i> Em estoque
                        </div>
                        <button class="w-full bg-purple-600 text-white py-2 rounded-lg hover:bg-purple-700 transition">
                            <i class="fas fa-cart-plus mr-2"></i> Comprar
                        </button>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-8">
                <button class="bg-purple-600 text-white px-6 py-3 rounded-lg font-bold hover:bg-purple-700 transition">
                    Ver Todos os Produtos
                </button>
            </div>
        </div>
    </section>

    <!-- Brands -->
    <section class="py-8 bg-gray-100">
        <div class="container mx-auto px-4">
            <h3 class="text-2xl font-bold mb-6 text-gray-800 text-center">Marcas Parceiras</h3>
            
            <div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-6 gap-6">
                <div class="bg-white p-6 rounded-lg flex items-center justify-center">
                    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/ae/AMD_logo_2017.svg/2560px-AMD_logo_2017.svg.png" alt="AMD" class="h-12 object-contain">
                </div>
                <div class="bg-white p-6 rounded-lg flex items-center justify-center">
                    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/7d/Intel_logo_%282006-2020%29.svg/2560px-Intel_logo_%282006-2020%29.svg.png" alt="Intel" class="h-12 object-contain">
                </div>
                <div class="bg-white p-6 rounded-lg flex items-center justify-center">
                    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fa/NVIDIA_logo.svg/2560px-NVIDIA_logo.svg.png" alt="NVIDIA" class="h-12 object-contain">
                </div>
                <div class="bg-white p-6 rounded-lg flex items-center justify-center">
                    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/24/Samsung_Logo.svg/2560px-Samsung_Logo.svg.png" alt="Samsung" class="h-12 object-contain">
                </div>
                <div class="bg-white p-6 rounded-lg flex items-center justify-center">
                    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8d/ASUS_Logo.svg/2560px-ASUS_Logo.svg.png" alt="ASUS" class="h-12 object-contain">
                </div>
                <div class="bg-white p-6 rounded-lg flex items-center justify-center">
                    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/96/Microsoft_logo_%282012%29.svg/2560px-Microsoft_logo_%282012%29.svg.png" alt="Microsoft" class="h-12 object-contain">
                </div>
            </div>
        </div>
    </section>

    <!-- Newsletter -->
    <section class="py-12 bg-purple-700 text-white">
        <div class="container mx-auto px-4 text-center">
            <h3 class="text-3xl font-bold mb-4">Receba nossas ofertas</h3>
            <p class="text-xl mb-6 max-w-2xl mx-auto">Cadastre-se e receba as melhores promoções e novidades do Instituto Café diretamente no seu e-mail.</p>
            
            <div class="max-w-md mx-auto">
                <div class="flex">
                    <input type="email" placeholder="Seu melhor e-mail" class="flex-1 px-4 py-3 rounded-l-lg focus:outline-none text-gray-900">
                    <button class="bg-purple-900 px-6 py-3 rounded-r-lg font-bold hover:bg-purple-800 transition">
                        Cadastrar
                    </button>
                </div>
                <div class="mt-2 text-sm">
                    <label class="flex items-center justify-center">
                        <input type="checkbox" class="mr-2">
                        <span>Concordo em receber comunicações do Instituto Café</span>
                    </label>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white pt-12 pb-6">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8 mb-8">
                <!-- About -->
                <div>
                    <h4 class="text-xl font-bold mb-4 flex items-center">
                        <div class="coffee-icon text-2xl text-purple-500 mr-2">
                            <i class="fas fa-coffee"></i>
                        </div>
                        Instituto Café
                    </h4>
                    <p class="text-gray-400 mb-4">Tecnologia com sabor e qualidade para você aproveitar o melhor do mundo digital.</p>
                    <div class="flex space-x-4">
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-twitter"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                
                <!-- Links -->
                <div>
                    <h4 class="text-lg font-bold mb-4">Institucional</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white">Quem Somos</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Nossas Lojas</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Política de Privacidade</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Termos de Uso</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Trabalhe Conosco</a></li>
                    </ul>
                </div>
                
                <!-- Help -->
                <div>
                    <h4 class="text-lg font-bold mb-4">Ajuda</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white">Central de Atendimento</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Como Comprar</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Frete e Entrega</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Trocas e Devoluções</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Dúvidas Frequentes</a></li>
                    </ul>
                </div>
                
                <!-- Contact -->
                <div>
                    <h4 class="text-lg font-bold mb-4">Contato</h4>
                    <ul class="space-y-2 text-gray-400">
                        <li class="flex items-start">
                            <i class="fas fa-map-marker-alt mt-1 mr-2"></i>
                            <span>Av. Paulista, 1000 - São Paulo/SP</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-phone-alt mr-2"></i>
                            <span>(11) 4002-8922</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-envelope mr-2"></i>
                            <span>contato@institutocafe.com.br</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-clock mr-2"></i>
                            <span>Seg a Sex: 9h às 18h</span>
                        </li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-gray-800 pt-6">
                <div class="flex flex-col md:flex-row justify-between items-center">
                    <div class="text-gray-400 text-sm mb-4 md:mb-0">
                        &copy; 2023 Instituto Café. Todos os direitos reservados.
                    </div>
                    <div class="flex space-x-4">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5e/Visa_Inc._logo.svg/2560px-Visa_Inc._logo.svg.png" alt="Visa" class="h-6">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/2a/Mastercard-logo.svg/1280px-Mastercard-logo.svg.png" alt="Mastercard" class="h-6">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/32/American_Express_logo.svg/1280px-American_Express_logo.svg.png" alt="American Express" class="h-6">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/bb/Elo_logo.svg/1200px-Elo_logo.svg.png" alt="Elo" class="h-6">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f0/Pix_logo.svg/1200px-Pix_logo.svg.png" alt="Pix" class="h-6">
                    </div>
                </div>
            </div>
        </div>
    </footer>

    <!-- WhatsApp Button -->
    <div class="fixed bottom-6 right-6 z-50">
        <a href="#" class="bg-green-500 text-white p-3 rounded-full shadow-lg hover:bg-green-600 transition flex items-center justify-center">
            <i class="fab fa-whatsapp text-2xl"></i>
        </a>
    </div>

    <script>
        // Countdown timer for flash deal
        function updateCountdown() {
            const now = new Date();
            const endOfDay = new Date();
            endOfDay.setHours(23, 59, 59, 0);
            
            const diff = endOfDay - now;
            
            const hours = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((diff % (1000 * 60)) / 1000);
            
            document.getElementById('countdown').textContent = 
                `${hours.toString().padStart(2, '0')}:${minutes.toString().padStart(2, '0')}:${seconds.toString().padStart(2, '0')}`;
        }
        
        setInterval(updateCountdown, 1000);
        updateCountdown();
        
        // Simple product hover effect
        document.querySelectorAll('.product-card').forEach(card => {
            card.addEventListener('mouseenter', () => {
                card.style.transition = 'transform 0.3s ease, box-shadow 0.3s ease';
            });
        });
    </script>
</body>
</html>
