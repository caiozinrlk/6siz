<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>6siz ScreenShare</title>
    <link rel="icon" type="image/png" href="./public/assets/gengar.png">
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
<script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
<script>
    document.addEventListener('DOMContentLoaded', function () {
        AOS.init();
    });
</script>

    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap');
        body {
            font-family: 'Inter', sans-serif;
        }

        /* Fundo com partículas animadas */
        .background-animation {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            z-index: -1;
        }

        .background-animation div {
            position: absolute;
            width: 5px;
            height: 5px;
            background: rgba(0, 247, 255, 0.8);
            border-radius: 50%;
            animation: move 10s infinite ease-in-out;
        }

        @keyframes move {
            0% {
                transform: translateY(0) translateX(0);
            }
            50% {
                transform: translateY(100vh) translateX(100vw);
            }
            100% {
                transform: translateY(0) translateX(0);
            }
        }
        /* Estilo das bandeiras */
        .language-switcher {
            position: fixed;
            top: 1rem;
            right: 1rem;
            z-index: 50;
            display: flex;
            gap: 0.5rem;
        }

        .language-switcher img {
            width: 30px;
            height: 20px;
            cursor: pointer;
            border-radius: 3px;
            transition: transform 0.2s ease;
        }

        .language-switcher img:hover {
            transform: scale(1.1);
        }
    </style>
    <style>
            /* Discord Icon Styling */
            .discord-icon {
                position: fixed;
                top: 1rem;
                left: 1rem;
                z-index: 50;
                width: 40px;
                height: 40px;
                cursor: pointer;
                transition: filter 0.3s ease;
                filter: grayscale(1);
            }
    
            .discord-icon:hover {
                filter: grayscale(0);
            }
    
            /* Partner Logos Hover Effect */
            .partner-logo {
                transition: transform 0.3s ease, filter 0.3s ease;
                filter: grayscale(1);
            }
    
            .partner-logo:hover {
                transform: scale(1.1);
                filter: grayscale(0);
            }
        </style>
</head>
<body class="relative bg-black text-white">
    <a href="https://discord.gg/kBAHaNbqYH" target="_blank">
        <img src="https://support.discord.com/hc/user_images/bbW4u80g7yIVxsphv9diNw.png" 
             alt="Discord" 
             class="discord-icon">
    </a>

    <!-- Bandeiras para alternar idioma -->
    <div class="language-switcher">
        <img src="https://flagcdn.com/w320/br.png" alt="Português" id="btn-pt" title="Português">
        <img src="https://flagcdn.com/w320/us.png" alt="English" id="btn-en" title="English">
    </div>

    <!-- Animações de fundo -->
    <div class="background-animation">
        <div style="top: 20%; left: 15%; animation-duration: 14s;"></div>
        <div style="top: 50%; left: 30%; animation-duration: 10s;"></div>
        <div style="top: 70%; left: 60%; animation-duration: 12s;"></div>
        <div style="top: 40%; left: 80%; animation-duration: 16s;"></div>
    </div>

    <!-- Cabeçalho -->
    <header class="bg-opacity-50 bg-black py-6 fixed top-0 w-full z-10">
        <div class="container mx-auto flex items-center justify-between px-6">
            <!-- Navegação Lado Esquerdo -->
            <nav class="flex space-x-4">
                <a href="#partners" class="text-gray-300 hover:text-purple-600" 
                   data-pt="Parceiros" data-en="Partners">Parceiros</a>
                <a href="#feedbacks" class="text-gray-300 hover:text-purple-600" data-pt="Feedbacks" data-en="Reviews">Feedbacks</a>
                <a href="#pricing" class="text-gray-300 hover:text-purple-600" 
                   data-pt="Preços" data-en="Pricing">Preços</a>
                </nav>
    
            <!-- GIF Centralizado -->
            <div class="flex justify-center items-center">
                <img src="https://cdn.discordapp.com/attachments/1336455368166866944/1337229196812095559/pngtree-cartoon-ghost-for-halloween-png-image_13395839-removebg-preview.png?ex=67a757fd&is=67a6067d&hm=7734ef0a3a33c656c1523599732dcd59324416fa01168ac50237b9871127ff3a&.gif" alt="Gengar GIF" class="h-12">
            </div>
    
            <!-- Navegação Lado Direito -->
            <nav class="flex space-x-4 items-center">
                    <a href="https://discord.gg/kBAHaNbqYH" 
                   class="group relative inline-block px-6 py-2 font-bold text-lg rounded-lg overflow-hidden ring-[2px] ring-neutral-900 text-gray-300 transition-colors duration-200 hover:text-purple-300" 
                   data-pt="Login" 
                   data-href-pt="https://discord.gg/kBAHaNbqYH" 
                   data-en="Login" 
                   data-href-en="https://discord.gg/kBAHaNbqYH">
                   <span class="absolute inset-0 h-full w-full overflow-hidden rounded-full mask-gradient">
                        <span class="animate-flip before:animate-kitrotate absolute inset-0 h-full w-full overflow-hidden rounded-full [mask:linear-gradient(white,_transparent_50%)] 
                                     before:absolute before:aspect-square before:w-[200%] before:rotate-[-90deg] 
                                     before:bg-[conic-gradient(from_0deg,transparent_0_340deg,white_360deg)] 
                                     before:content-[''] before:[inset:0_auto_auto_50%] before:[translate:-50%_-15%]">
                        </span>
                    </span>
                    <!-- Fundo de Transição -->
                    <span class="backdrop absolute inset-px rounded-full bg-gradient-to-r from-gray-950 to-black transition-colors duration-200"></span>
                    <!-- Texto do Botão -->
                    <span class="relative z-10 text-white">Login</span></a>
                   
                   <a href="https://discord.gg/kBAHaNbqYH" 
                   class="group relative inline-block px-6 py-2 font-bold text-lg rounded-lg overflow-hidden ring-[2px] ring-neutral-900 text-gray-300 transition-colors duration-200 hover:text-purple-300" 
                   data-pt="Compre Agora" 
                   data-href-pt="https://discord.gg/kBAHaNbqYH" 
                   data-en="Buy Now" 
                   data-href-en="https://discord.gg/kBAHaNbqYH">
                    <!-- Efeito Neon -->
                    <span class="absolute inset-0 h-full w-full overflow-hidden rounded-full mask-gradient">
                        <span class="animate-flip before:animate-kitrotate absolute inset-0 h-full w-full overflow-hidden rounded-full [mask:linear-gradient(white,_transparent_50%)] 
                                     before:absolute before:aspect-square before:w-[200%] before:rotate-[-90deg] 
                                     before:bg-[conic-gradient(from_0deg,transparent_0_340deg,white_360deg)] 
                                     before:content-[''] before:[inset:0_auto_auto_50%] before:[translate:-50%_-15%]">
                        </span>
                    </span>
                    <!-- Fundo de Transição -->
                    <span class="backdrop absolute inset-px rounded-full bg-gradient-to-r from-gray-950 to-black transition-colors duration-200"></span>
                    <!-- Texto do Botão -->
                    <span class="relative z-10 text-white">Compre Agora</span>
                </a>
            </nav>
        </div>
    </header>

    <section class="h-screen flex items-center justify-center text-center relative overflow-hidden bg-black">
        <!-- Fundo com linhas de quadrados -->
        <div class="absolute inset-0 w-full h-full bg-grid z-0"></div>
    
        <!-- Canvas para partículas DNA -->
        <canvas id="dnaCanvas" class="absolute inset-0 w-full h-full"></canvas>
    
        <!-- Conteúdo -->
        <div class="relative z-10">
            <h1 id="typing-effect" class="text-6xl md:text-7xl font-extrabold text-transparent bg-clip-text animate-pulse"></h1>
            <p class="text-xl text-gray-400 mt-4">
                <span data-pt="Experiência única de aprender com os melhores" data-en="A unique experience of learning from the best">Experiência única de aprender com os melhores</span>
                <span data-pt="para se tornar um deles." data-en="to become one of them.">para se tornar um deles.</span>
            </p>
            <a href="#features" 
               class="mt-8 inline-block bg-purple-500 hover:bg-purple-600 text-white py-3 px-8 rounded-lg text-lg font-bold shadow-lg"
               data-pt="Conheça Agora" data-en="Get Started">Conheça Agora</a>
            
            
            <!-- Estilos -->
            <style>
                /* Efeito de pulsação com gradiente */
                @keyframes pulse {
                    0%, 100% {
                        background-size: 300%; /* Define o gradiente inicial */
                        transform: scale(1); /* Tamanho normal */
                    }
                    50% {
                        background-size: 400%; /* Expande ligeiramente o gradiente */
                        transform: scale(1.05); /* Tamanho maior */
                    }
                }
                @keyframes kitrotate {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}

.animate-kitrotate {
  animation: kitrotate 3s linear infinite;
}

@keyframes flip {
  0%, 100% {
    transform: rotateY(0deg);
  }
  50% {
    transform: rotateY(180deg);
  }
}

.animate-flip {
  animation: flip 2s linear infinite;
}

            
                .animate-pulse {
                    background-image: linear-gradient(
                        90deg,
                        #00f7ff,
                        #003cff,
                        #00f7ff,
                        #0400ff,
                        #00f7ff,
                        #1100ff
                    );
                    background-size: 300%; /* Gradiente contínuo */
                    animation: pulse 1s infinite; /* Efeito de pulsação */
                    background-clip: text;
                    -webkit-background-clip: text;
                    color: transparent; /* Esconde a cor original do texto */
                }
            </style>
            
    
        <!-- Estilo -->
        <style>
          /* Estilo do container dos cartões */
.price-card-container {
  display: flex;
  justify-content: center;
  align-items: flex-end;
  gap: 1.5rem;
}

/* Cartões laterais */
.price-card {
  flex: 1; /* Tamanho padrão */
  transform: scale(0.95); /* Reduz o tamanho */
  transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

.price-card:hover {
  transform: scale(1); /* Aumenta levemente ao passar o mouse */
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.4);
}

/* Cartão central (destacado) */
.price-card.featured {
  flex: 1.2; /* Maior proporção */
  transform: scale(1.1); /* Destaca o tamanho */
  z-index: 10; /* Garante que fique sobreposto */
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.4);
  transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
}

.price-card.featured:hover {
  transform: scale(1.15); /* Destaca ainda mais ao passar o mouse */
}


            /* Estilo para o container do carrossel */
            .marquee {
              display: flex;
              overflow: hidden;
              position: relative;
              width: 100%;
              margin-bottom: 3rem; /* Espaçamento entre os carrosséis */
            }
          
            .marquee .track {
              display: flex;
              animation: scroll var(--duration) linear infinite;
              gap: 2rem; /* Espaçamento horizontal entre os cards */
            }
          
            .marquee.reverse .track {
              animation-direction: reverse;
            }
          
            @keyframes scroll {
              0% {
                transform: translateX(0);
              }
              100% {
                transform: translateX(-50%);
              }
            }
          
            /* Estilo dos cards de feedback */
            .review-card {
              flex-shrink: 0;
              width: 280px;
              height: auto;
              background: linear-gradient(145deg, #222, #1a1a1a); /* Gradiente sutil */
              border: 1px solid rgba(255, 255, 255, 0.1); /* Borda sutil */
              border-radius: 12px; /* Cantos arredondados */
              padding: 20px;
              box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3); /* Sombra discreta */
              display: flex;
              flex-direction: column;
              align-items: center;
              justify-content: space-between;
              color: #f0f0f0; /* Cor do texto mais clara */
              transition: transform 0.3s ease, box-shadow 0.3s ease;
            }
          
            /* Efeito de hover para os cards */
            .review-card:hover {
              transform: scale(1.05); /* Efeito de ampliação ao passar o mouse */
              box-shadow: 0 8px 16px rgba(0, 0, 0, 0.5); /* Sombra mais forte */
            }
          
            /* Imagem do autor do feedback */
            .review-card img {
              width: 60px;
              height: 60px;
              border-radius: 50%; /* Imagem circular */
              border: 2px solid #46bdc1; /* Borda roxa ao redor da imagem */
              margin-bottom: 12px;
            }
          
            /* Nome do autor */
            .review-card h3 {
              margin: 8px 0;
              font-size: 16px;
              font-weight: bold;
              color: #e0e0e0; /* Texto com contraste mais suave */
            }
          
            /* Texto do feedback */
            .review-card p {
              font-size: 14px;
              text-align: center;
              line-height: 1.5; /* Melhor espaçamento entre linhas */
              color: #cfcfcf; /* Texto mais claro */
            }
          </style>
          <style>
      @keyframes neon-border {
        0% {
          background-position: 0 0;
        }
        100% {
          background-position: 200% 0;
        }
      }
  
      /* Classe para criar a borda animada */
      .neon-worm-border {
        position: relative;
        border-radius: 12px; /* Bordas arredondadas */
        z-index: 1; /* Garante que o conteúdo fique acima */
        overflow: hidden; /* Esconde partes extras da borda */
      }
  
      .neon-worm-border::before {
        content: '';
        position: absolute;
        inset: 0; /* Expande para cobrir todo o elemento */
        border-radius: 12px;
        padding: 4px; /* Define a largura da borda */
        background: linear-gradient(
          90deg,
          #5cdff6,
          #8bd7fa,
          #01c2c9,
          #5c73f6
        ); /* Gradiente neon */
        background-size: 200% 200%; /* Expande o gradiente para animação */
        animation: neon-border 1s linear infinite; /* Anima o gradiente */
        -webkit-mask: linear-gradient(#fff 0 0) content-box, linear-gradient(#fff 0 0);
        mask: linear-gradient(#fff 0 0) content-box, linear-gradient(#fff 0 0);
        -webkit-mask-composite: destination-out;
        mask-composite: exclude; /* Faz a borda visível, mas não o fundo */
        z-index: -1; /* Mantém a borda atrás do conteúdo */
      }
    </style>
<style>
            /* Canvas para partículas */
            canvas {
                position: absolute;
                top: 0;
                left: 0;
                z-index: 0;
            }
    
            /* Fundo com linhas de quadrados */
            .bg-grid {
                background-color: black;
                background-image: linear-gradient(90deg, rgba(128, 128, 128, 0.2) 1px, transparent 1px),
                                  linear-gradient(180deg, rgba(128, 128, 128, 0.2) 1px, transparent 1px);
                background-size: 50px 50px; /* Tamanho das células */
            }
        </style>
    
        <!-- Script para partículas DNA -->
        <script>
            const canvas = document.getElementById('dnaCanvas');
            const ctx = canvas.getContext('2d');
    
            canvas.width = window.innerWidth;
            canvas.height = window.innerHeight;
    
            let particlesArray = [];
            const numberOfParticles = 150;
    
            // Classe Partícula
            class Particle {
                constructor(x, y, size, color, speedX, speedY) {
                    this.x = x;
                    this.y = y;
                    this.size = size;
                    this.color = color;
                    this.speedX = speedX;
                    this.speedY = speedY;
                }
                draw() {
                    ctx.beginPath();
                    ctx.arc(this.x, this.y, this.size, 0, Math.PI * 2);
                    ctx.fillStyle = this.color;
                    ctx.fill();
                }
                update() {
                    this.x += this.speedX;
                    this.y += this.speedY;
    
                    // Reaparecer no topo ao sair da tela
                    if (this.y > canvas.height) {
                        this.y = 0 - this.size;
                        this.x = Math.random() * canvas.width;
                    }
                }
            }
    
            // Criar Partículas
            function init() {
                particlesArray = [];
                for (let i = 0; i < numberOfParticles; i++) {
                    const size = Math.random() * 2 + 1;
                    const x = Math.random() * canvas.width;
                    const y = Math.random() * canvas.height;
                    const color = `rgba(128, 0, 255, 0.8)`;
                    const speedX = Math.random() * 0.5 - 0.25;
                    const speedY = Math.random() * 0.5 + 0.5;
                    particlesArray.push(new Particle(x, y, size, color, speedX, speedY));
                }
            }
    
            // Animação
            function animate() {
                ctx.clearRect(0, 0, canvas.width, canvas.height);
    
                // Desenhar DNA com partículas
                particlesArray.forEach((particle, index) => {
                    particle.update();
                    particle.draw();
    
                    // Conectar partículas para criar "hélices"
                    for (let j = index; j < particlesArray.length; j++) {
                        const dx = particle.x - particlesArray[j].x;
                        const dy = particle.y - particlesArray[j].y;
                        const distance = Math.sqrt(dx * dx + dy * dy);
    
                        if (distance < 80) {
                            ctx.beginPath();
                            ctx.strokeStyle = `rgba(128, 0, 255, ${1 - distance / 80})`;
                            ctx.lineWidth = 0.5;
                            ctx.moveTo(particle.x, particle.y);
                            ctx.lineTo(particlesArray[j].x, particlesArray[j].y);
                            ctx.stroke();
                        }
                    }
                });
    
                requestAnimationFrame(animate);
            }
    
            // Ajustar ao redimensionar
            window.addEventListener('resize', () => {
                canvas.width = window.innerWidth;
                canvas.height = window.innerHeight;
                init();
            });
    
            // Inicializar
            init();
            animate();
        </script>
    </section>
    
       
    
        <section id="feedbacks" class="py-10 bg-black text-white" data-aos="fade-up" data-aos-duration="1800">
        <div class="container mx-auto text-center px-6">
          <!-- Título -->
          <h3 class="text-3xl font-bold text-purple-300 mb-8" data-pt="Feedbacks" data-en="Reviews">Feedbacks</h3>
        </div>
      
        <!-- Carrossel de feedbacks -->
        <div class="marquee" style="--duration: 30s">
          <div class="track">
            <!-- Primeira fileira de feedbacks -->
            <div class="review-card">
              <img src="https://cdn.discordapp.com/attachments/1279197824436797526/1337387732720156742/D3E7CA1B-A12D-4F6B-9C6E-8BA41D7C0A17.jpg?ex=67a742e2&is=67a5f162&hm=88965b8aa6bea2df5e83ac3bf26b8c351e4bc458b773d7ce35b69b023b93f7f3&" alt="Jota Jesus" />
              <h3>ricardo <span class="text-purple-400">@ricardo157</span></h3>
              <p>Venho te agradecer pelo aprendizado e por te ajudado a conquista essa nova experiência...</p>
            </div>
            <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/940989282674413638/e463098a152bde1aa45d162004c2f44a.webp?size=1024" alt="Z7" />
              <h3>Z7 <span class="text-purple-400">@Z7</span></h3>
              <p>Slk graças ao @6siz consegue pegar uma experiência que jamais achei que conseguiria...</p>
            </div>
            <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/1260345159896268800/a_9ef0597b10dfc8a3d06cdded06c3152f.gif?size=1024" alt="The Ripper" />
              <h3>The Ripper <span class="text-purple-400">@TheRipper</span></h3>
              <p>Slk graças ao @purple consegui entrar pra equipe de SS, coisa que sempre quis...</p>
            </div>
            <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/444844686171963393/a_7d6374448b8e63a3ac513fb2e74eb3ee.gif?size=1024" alt="Du" />
              <h3>Du <span class="text-purple-400">@Du</span></h3>
              <p>Papai @purple explica muito bem, tudo bem detalhado e com exemplos reais! Aprendi a telar muito rápido.</p>
            </div>
            <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/279764357175443457/a4aaad0b669102d1c6109d8c2576dfc3.webp?size=1024&format=webp" alt="Kauntzz" />
              <h3>Kauntzz <span class="text-purple-400">@Kauntzz</span></h3>
              <p>muito bom cara, comecei na telagem do 0 e agr to de SS na nobre, o cara é brabo na didatica!</p>
            </div>
            <div class="review-card">
                <img src="https://cdn.discordapp.com/avatars/329856602431815689/058d9cc58980a710d008b6f80103e16f.webp?size=1024&format=webp" alt="LCS" />
                <h3>LC$ <span class="text-purple-400">@LCS1single</span></h3>
                <p>Ótimo curso, aulas bem detalhadas e suporte excelente</p>
              </div>
              <div class="review-card">
                <img src="https://cdn.discordapp.com/avatars/1128419903137919027/31d66064d8267ee31b39696035605b5d.webp?size=1024&format=webp" alt="Juliax11" />
                <h3>Julia <span class="text-purple-400">@juliax11</span></h3>
                <p>Ótimo curso,muito  explicativo, parabens pelo curso purple</p>
              </div>
              <div class="review-card">
                <img src="https://images-ext-1.discordapp.net/external/WaZhFV5zAZFfw1HHy-HzLyw03UbwOENOjTyQqmIlYSU/%3Fsize%3D2048/https/cdn.discordapp.com/avatars/346828678648299532/a_3b6c567068774609da2664867bcc41d4.gif" alt="YanDecker" />
                <h3>YanDecker <span class="text-purple-400">@yannzinn</span></h3>
                <p>Curso muito bom tive uma experiência muito foda comecei a telar por causa do curso e muitos foi de vasco</p>
              </div>
              <div class="review-card">
                <img src="https://images-ext-1.discordapp.net/external/5MIuF9VTAh5DxplxGDzF6zJQkRt4iFFFFBs0wZxK0ss/%3Fsize%3D2048/https/cdn.discordapp.com/avatars/338184665896583178/9d192a04e7f3ac67ead6452c0ca8fa69.png" alt="Yuna" />
                <h3>Yuna <span class="text-purple-400">@YunaNobre</span></h3>
                <p>Peguei altos bypass, muito bom nota deix</p>
              </div>
            <div class="review-card">
                <img src="https://cdn.discordapp.com/avatars/940989282674413638/ecc7b57951fdb2df3a8c9bba86768faf.webp?size=1024" alt="T7 AQUA" />
                <h3>T7 AQUA <span class="text-purple-400">@T7AQUA</span></h3>
                <p>Curso muito foda papo reto, aprendi muita coisa e aprendo muito com esse curso...</p>
              </div>
                          <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/184713609035644928/0570efba5cfbc0ead1a64a8d034bfbd8.webp?size=1024" alt="Jota Jesus" />
              <h3>Jota Jesus <span class="text-purple-400">@JotaJesus</span></h3>
              <p>Venho te agradecer pelo aprendizado e por te ajudado a conquista essa nova experiência...</p>
            </div>
            <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/940989282674413638/e463098a152bde1aa45d162004c2f44a.webp?size=1024" alt="Z7" />
              <h3>Z7 <span class="text-purple-400">@Z7</span></h3>
              <p>Slk graças ao @purple consegue pegar uma experiência que jamais achei que conseguiria...</p>
            </div>
            <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/1260345159896268800/a_9ef0597b10dfc8a3d06cdded06c3152f.gif?size=1024" alt="The Ripper" />
              <h3>The Ripper <span class="text-purple-400">@TheRipper</span></h3>
              <p>Slk graças ao @purple consegui entrar pra equipe de SS, coisa que sempre quis...</p>
            </div>
            <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/444844686171963393/a_7d6374448b8e63a3ac513fb2e74eb3ee.gif?size=1024" alt="Du" />
              <h3>Du <span class="text-purple-400">@Du</span></h3>
              <p>Papai @purple explica muito bem, tudo bem detalhado e com exemplos reais! Aprendi a telar muito rápido.</p>
            </div>
            <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/279764357175443457/a4aaad0b669102d1c6109d8c2576dfc3.webp?size=1024&format=webp" alt="Kauntzz" />
              <h3>Kauntzz <span class="text-purple-400">@Kauntzz</span></h3>
              <p>muito bom cara, comecei na telagem do 0 e agr to de SS na nobre, o cara é brabo na didatica!</p>
            </div>
            <div class="review-card">
                <img src="https://cdn.discordapp.com/avatars/329856602431815689/058d9cc58980a710d008b6f80103e16f.webp?size=1024&format=webp" alt="LCS" />
                <h3>LC$ <span class="text-purple-400">@LCS1single</span></h3>
                <p>Ótimo curso, aulas bem detalhadas e suporte excelente</p>
              </div>
              <div class="review-card">
                <img src="https://cdn.discordapp.com/avatars/1128419903137919027/31d66064d8267ee31b39696035605b5d.webp?size=1024&format=webp" alt="Juliax11" />
                <h3>Julia <span class="text-purple-400">@juliax11</span></h3>
                <p>Ótimo curso,muito  explicativo, parabens pelo curso purple</p>
              </div>
              <div class="review-card">
                <img src="https://images-ext-1.discordapp.net/external/WaZhFV5zAZFfw1HHy-HzLyw03UbwOENOjTyQqmIlYSU/%3Fsize%3D2048/https/cdn.discordapp.com/avatars/346828678648299532/a_3b6c567068774609da2664867bcc41d4.gif" alt="YanDecker" />
                <h3>YanDecker <span class="text-purple-400">@yannzinn</span></h3>
                <p>Curso muito bom tive uma experiência muito foda comecei a telar por causa do curso e muitos foi de vasco</p>
              </div>
              <div class="review-card">
                <img src="https://images-ext-1.discordapp.net/external/5MIuF9VTAh5DxplxGDzF6zJQkRt4iFFFFBs0wZxK0ss/%3Fsize%3D2048/https/cdn.discordapp.com/avatars/338184665896583178/9d192a04e7f3ac67ead6452c0ca8fa69.png" alt="Yuna" />
                <h3>Yuna <span class="text-purple-400">@YunaNobre</span></h3>
                <p>Peguei altos bypass, muito bom nota deix</p>
              </div>
            <div class="review-card">
                <img src="https://cdn.discordapp.com/avatars/940989282674413638/ecc7b57951fdb2df3a8c9bba86768faf.webp?size=1024" alt="T7 AQUA" />
                <h3>T7 AQUA <span class="text-purple-400">@T7AQUA</span></h3>
                <p>Curso muito foda papo reto, aprendi muita coisa e aprendo muito com esse curso...</p>
              </div>
                <div class="review-card">
                  <img src="https://cdn.discordapp.com/avatars/940989282674413638/ecc7b57951fdb2df3a8c9bba86768faf.webp?size=1024" alt="ygor.rlk" />
                  <h3>ygor.rlk<span class="text-purple-400">ygor.rlk</span></h3>
                  <p>Slk Purple viado seu curso e vc é pika mo transparência gostei pá pohaaa do curso e 3 dias eu já sei o básico sobre telagem agradeço desde de já</p>
                  </div>
                <div class="review-card">
                  <img src="https://cdn.discordapp.com/avatars/1055997116364902490/0fe4efc76c86c9f6c983c1c1f69e3f04.webp?size=1024" alt="Guga" />
                  <h3>Guga<span class="text-purple-400">Guga</span></h3>
                  <p>melhor curso q ta tendo.</p>
                </div>
            </div>
              </div>
        <div class="marquee reverse" style="--duration: 30s">
          <div class="track">
            <!-- Segunda fileira de feedbacks -->
            <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/1156711887816376330/2320e8d59ef02164576e4afd799b0ddb.webp?size=1024" alt="vint3zada" />
              <h3>vint3zada <span class="text-purple-400">@vint3zada</span></h3>
              <p>Curso muito foda, estou no ensino básico ainda mas já gravei muitas coisas...</p>
            </div>
            <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/1160411238610763858/20de37c7c9fc244ef162d0e35d3935a1.webp?size=1024" alt="Yuni dos Fatos" />
              <h3>Yuni dos Fatos <span class="text-purple-400">@YuniNobre</span></h3>
              <p>Curso muito bom, vale muita pena, recomendo bastante caso alguém tenha dúvida...</p>
            </div>
            <div class="review-card">
                <img src="https://cdn.discordapp.com/avatars/866405402878804018/0ea1507e1ddd33de9d5577adc5b84c27.webp?size=1024" alt="blue" />
                <h3>slv <span class="text-purple-400">@0skdaw</span></h3>
                <p>Pprt curso que me introduziu no mundo da screenshare do fivem Graças ao mano Purple que eu aprendi a pegar bypass e dar exe na cara</p>
              </div>
            <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/1273620035482423351/cf87bd2fc55c1f16ff226bf3e3c7efd3.webp?size=1024" alt="blue" />
              <h3>blue <span class="text-purple-400">@bluesouza</span></h3>
              <p>Curso muito bom, recomendo muito, ensinou muito que até hoje sou resp ss da nobre...</p>
            </div>
            <div class="review-card">
                <img src="https://cdn.discordapp.com/avatars/866405402878804018/0ea1507e1ddd33de9d5577adc5b84c27.webp?size=1024" alt="blue" />
                <h3>slv <span class="text-purple-400">@0skdaw</span></h3>
                <p>Pprt curso que me introduziu no mundo da screenshare do fivem Graças ao mano Purple que eu aprendi a pegar bypass e dar exe na cara</p>
              </div>
            <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/1281064370516004885/2e90cafeefa69b30b2ad2f19c70384c2.webp?size=1024" alt="f" />
              <h3>f <span class="text-purple-400">@fpinsane</span></h3>
              <p>Slc melhor curso que eu já fiz, recomendo muito 1000000000/10 o melhor professor!</p>
            </div>
            <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/1184653608562741268/a8a05245653e2db4d98b8ec3ef7b577c.webp?size=1024" alt="Abu" />
              <h3>Abu <span class="text-purple-400">@Abuuzera</span></h3>
              <p>Curso Ótimo ajuda muito pois sempre explica direitinho ainda mais a aula 6 que chegou explicando tudo tirando a dúvida</p>
            </div>
            <div class="review-card">
                <img src="https://cdn.discordapp.com/avatars/1277760649610526781/e9782689f19077045c533aafda39cfe5.webp?size=1024" alt="HBT" />
                <h3>HBT <span class="text-purple-400">@HBTNobre</span></h3>
                <p>Curso muito bom, aqui eu aprendi a telar de verdade graças ao professor @purple...</p>
              </div>
              <div class="review-card">
                <img src="https://cdn.discordapp.com/avatars/472961261840236545/a_8c261127291fc350529236284338e7fc.gif?size=1024" alt="Ronald" />
                <h3>Ronald <span class="text-purple-400">@ronald77</span></h3>
                <p>10/10 - O melhor que temos né @purple , ele msm nosso monstro, curso zika, forte abraço da minha parte</p>
              </div>
              <div class="review-card">
                <img src="https://cdn.discordapp.com/avatars/1184296527456383019/4c435627eedf9181aaf3dc5d3c10b0e5.webp?size=1024" alt="MT" />
                <h3>MT <span class="text-purple-400">@mtjogano7</span></h3>
                <p>curso ta na rajada tropa, 10/10 @purple menor é brb</p>
              </div>
              <div class="review-card">
                <img src="https://images-ext-1.discordapp.net/external/IW1ShIIiwJNVAhKfIuSJYs5TE1SgRsjR_bboDzo9cAk/%3Fsize%3D2048/https/cdn.discordapp.com/avatars/756660673265533028/f5d62039b72358e4a16564a71c337257.png" alt="Misko" />
                <h3>Misko <span class="text-purple-400">@misko7pta</span></h3>
                <p>bom de mais o curso aprendi muito com as aulas 100/10</p>
              </div>
              <div class="review-card">
                <img src="https://cdn.discordapp.com/avatars/1216460513429688504/897015dcd76b93d637f1c6a53c0c026b.webp?size=1024" alt="LarissaNatsumi" />
                <h3>Natsumi <span class="text-purple-400">@LarissaNatsumi</span></h3>
                <p>bom de mais esse curso apenas com as aulas gravadas ja aprendir muito 100/10</p>
              </div>
            <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/1156711887816376330/2320e8d59ef02164576e4afd799b0ddb.webp?size=1024" alt="vint3zada" />
              <h3>vint3zada <span class="text-purple-400">@vint3zada</span></h3>
              <p>Curso muito foda, estou no ensino básico ainda mas já gravei muitas coisas...</p>
            </div>
            <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/1160411238610763858/20de37c7c9fc244ef162d0e35d3935a1.webp?size=1024" alt="Yuni dos Fatos" />
              <h3>Yuni dos Fatos <span class="text-purple-400">@YuniNobre</span></h3>
              <p>Curso muito bom, vale muita pena, recomendo bastante caso alguém tenha dúvida...</p>
            </div>
            <div class="review-card">
                <img src="https://cdn.discordapp.com/avatars/866405402878804018/0ea1507e1ddd33de9d5577adc5b84c27.webp?size=1024" alt="blue" />
                <h3>slv <span class="text-purple-400">@0skdaw</span></h3>
                <p>Pprt curso que me introduziu no mundo da screenshare do fivem Graças ao mano Purple que eu aprendi a pegar bypass e dar exe na cara</p>
              </div>
            <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/1273620035482423351/cf87bd2fc55c1f16ff226bf3e3c7efd3.webp?size=1024" alt="blue" />
              <h3>blue <span class="text-purple-400">@bluesouza</span></h3>
              <p>Curso muito bom, recomendo muito, ensinou muito que até hoje sou resp ss da nobre...</p>
            </div>
            <div class="review-card">
                <img src="https://cdn.discordapp.com/avatars/866405402878804018/0ea1507e1ddd33de9d5577adc5b84c27.webp?size=1024" alt="blue" />
                <h3>slv <span class="text-purple-400">@0skdaw</span></h3>
                <p>Pprt curso que me introduziu no mundo da screenshare do fivem Graças ao mano Purple que eu aprendi a pegar bypass e dar exe na cara</p>
              </div>
            <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/1281064370516004885/2e90cafeefa69b30b2ad2f19c70384c2.webp?size=1024" alt="f" />
              <h3>f <span class="text-purple-400">@fpinsane</span></h3>
              <p>Slc melhor curso que eu já fiz, recomendo muito 1000000000/10 o melhor professor!</p>
            </div>
            <div class="review-card">
              <img src="https://cdn.discordapp.com/avatars/1184653608562741268/a8a05245653e2db4d98b8ec3ef7b577c.webp?size=1024" alt="Abu" />
              <h3>Abu <span class="text-purple-400">@Abuuzera</span></h3>
              <p>Curso Ótimo ajuda muito pois sempre explica direitinho ainda mais a aula 6 que chegou explicando tudo tirando a dúvida</p>
            </div>
            <div class="review-card">
                <img src="https://cdn.discordapp.com/avatars/1277760649610526781/e9782689f19077045c533aafda39cfe5.webp?size=1024" alt="HBT" />
                <h3>HBT <span class="text-purple-400">@HBTNobre</span></h3>
                <p>Curso muito bom, aqui eu aprendi a telar de verdade graças ao professor @purple...</p>
              </div>
              <div class="review-card">
                <img src="https://cdn.discordapp.com/avatars/472961261840236545/a_8c261127291fc350529236284338e7fc.gif?size=1024" alt="Ronald" />
                <h3>Ronald <span class="text-purple-400">@ronald77</span></h3>
                <p>10/10 - O melhor que temos né @purple , ele msm nosso monstro, curso zika, forte abraço da minha parte</p>
              </div>
              <div class="review-card">
                <img src="https://cdn.discordapp.com/avatars/1184296527456383019/4c435627eedf9181aaf3dc5d3c10b0e5.webp?size=1024" alt="MT" />
                <h3>MT <span class="text-purple-400">@mtjogano7</span></h3>
                <p>curso ta na rajada tropa, 10/10 @purple menor é brb</p>
              </div>
              <div class="review-card">
                <img src="https://images-ext-1.discordapp.net/external/IW1ShIIiwJNVAhKfIuSJYs5TE1SgRsjR_bboDzo9cAk/%3Fsize%3D2048/https/cdn.discordapp.com/avatars/756660673265533028/f5d62039b72358e4a16564a71c337257.png" alt="Misko" />
                <h3>Misko <span class="text-purple-400">@misko7pta</span></h3>
                <p>bom de mais o curso aprendi muito com as aulas 100/10</p>
              </div>
              <div class="review-card">
                <img src="https://cdn.discordapp.com/avatars/1216460513429688504/897015dcd76b93d637f1c6a53c0c026b.webp?size=1024" alt="LarissaNatsumi" />
                <h3>Natsumi <span class="text-purple-400">@LarissaNatsumi</span></h3>
                <p>bom de mais esse curso apenas com as aulas gravadas ja aprendir muito 100/10</p>
              </div>
            <div class="review-card">
                  <img src="https://cdn.discordapp.com/avatars/1169613832122007637/387c6fbd3225b9d0904ccc24b1cf45e5.webp?size=1024" alt="rickzzrlq" />
                  <h3>rickzzrlq<span class="text-purple-400">@rickkzrlq</span></h3>
                  <p>the best screnshare course of brasil</p>
                </div>
            <div class="review-card">
                  <img src="https://cdn.discordapp.com/avatars/1278831644475920405/8d106977aa3e813edad531ad5556c02d.webp?size=1024" alt="Bolacharlq" />
                  <h3>bolacharlq<span class="text-purple-400">@bolacharlq</span></h3>
                  <p>muito bom o curso tu é brabo, Purple gostei dms vale apena!</p>
                </div>
            </div>
      </section>


      <!-- Coluna da Imagem de Fundo (Direita) -->
      <div class="w-full lg:w-1/2 relative">
          <div class="absolute inset-0 bg-gradient-to-l from-black via-transparent to-black opacity-75"></div>
          <div class="relative h-full w-full overflow-hidden">
              <!-- Imagem de Fundo -->
              <img src="./backg.png" 
                   alt="Background" 
                   class="object-cover w-full h-auto scale-110">
              <!-- Efeito de Degradê na Parte Inferior -->
              <div class="absolute bottom-0 inset-x-0 h-32 bg-gradient-to-t from-black via-transparent to-transparent"></div>
          </div>
      </div>
  </div>
</section>



    <!-- Preços -->
    <section class="py-12">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <h2 class="text-3xl font-extrabold text-purple-700 text-center mb-8">Preços</h2>
        
        <div class="grid grid-cols-1 md:grid-cols-3">
          <!-- Freelancer Plan -->
          <div class="bg-gray-900 bg-opacity-40 rounded-lg shadow-lg p-6">
            <h3 class="text-lg font-extrabold text-purple-700 mb-4 text-center">Consultoria Lv. 1 🔎</h3>
            <p class="text-purple-300 mb-6 text-center">A cara do cliente depois que abrimos o bypass de 600 reais dele 😲😭</p>
            <div class="text-4xl font-extrabold text-purple-700 mb-4 text-center">R$60,00<span class="text-lg text-purple-300 font-medium">/lifetime</span></div>
            <ul class="mb-6 space-y-2">
              <li class="flex items-center text-purple-100">
                <svg class="w-5 h-5 text-indigo-600 mr-2" fill="currentColor" viewBox="0 0 20 20">
                  <path d="M16.707 5.293a1 1 0 010 1.414L8.414 15H6v-2.414l8.293-8.293a1 1 0 011.414 0z"></path>
                </svg>
                <span data-pt="Aprendizado ao vivo e suporte sempre que precisar" data-en="
                Live learning and support whenever you need it">Curso totalmente ao vivo com aulas quando quiser</span>
              </li>
              <li class="flex items-center text-purple-100">
                <svg class="w-5 h-5 text-indigo-600 mr-2" fill="currentColor" viewBox="0 0 20 20">
                  <path d="M16.707 5.293a1 1 0 010 1.414L8.414 15H6v-2.414l8.293-8.293a1 1 0 011.414 0z"></path>
                </svg>
                <span data-pt="Contato direto com professores do curso" data-en="Direct contact with course teachers">Contato direto com professores do curso tenha o melhor suporte do Brasil</span>
              </li>
              <li class="flex items-center text-purple-100">
                <svg class="w-5 h-5 text-indigo-600 mr-2" fill="currentColor" viewBox="0 0 20 20">
                  <path d="M16.707 5.293a1 1 0 010 1.414L8.414 15H6v-2.414l8.293-8.293a1 1 0 011.414 0z"></path>
                </svg>
                <span data-pt="Pacote de Strings atualizadas para Scanner" data-en="Strings Pack for Scanner">Pacote de Strings atualizadas e privada para Scanner GRÁTIS</span>
              </li>
              <li class="flex items-center text-purple-100">
                <svg class="w-5 h-5 text-indigo-600 mr-2" fill="currentColor" viewBox="0 0 20 20">
                  <path d="M16.707 5.293a1 1 0 010 1.414L8.414 15H6v-2.414l8.293-8.293a1 1 0 011.414 0z"></path>
                </svg>
                <span data-pt="Quer a verdade sobre essa consultoria? É do C%R&LH*" data-en="The most Insane Consultancy to PC Check">Quer a verdade sobre essa consultoria? É do C%R&LH*</span>
              </li>
            </ul>
            <a href="https://discord.gg/kBAHaNbqYH" 
            class="block bg-purple-800 text-white py-2 rounded-lg hover:bg-purple-900 text-center" 
            data-href-pt="https://discord.gg/kBAHaNbqYH" 
            data-pt="Comprar Agora" 
            data-en="Not Available Yet" 
            data-href-en="https://discord.gg/kBAHaNbqYH">Comprar Agora</a>
          </div>
  
          <!-- Startup Plan -->
<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="neon-worm-border bg-gray-900 bg-opacity-40 rounded-lg shadow-lg p-9">
        <h3 class="text-lg font-extrabold text-purple-700 mb-4 text-center">Curso Basico 🔥</h3>
        <p class="text-purple-300 mb-6 text-center">Vamos executar o cheat do xitadinho na cara dele bb? 😉😴</p>
        <div class="text-4xl font-extrabold text-purple-700 mb-4 text-center">R$40,00<span class="text-lg text-purple-300 font-medium">/lifetime</span></div>
        <ul class="mb-6 space-y-2">
          <li class="flex items-center text-purple-100">
            <svg class="w-5 h-5 text-indigo-600 mr-2" fill="currentColor" viewBox="0 0 20 20">
              <path d="M16.707 5.293a1 1 0 010 1.414L8.414 15H6v-2.414l8.293-8.293a1 1 0 011.414 0z"></path>
            </svg>
            <span data-pt="Curso do básico ao avançado" data-en="Basic to advanced course">Curso do básico ao avançado</span>
          </li>
          <li class="flex items-center text-purple-100">
            <svg class="w-5 h-5 text-indigo-600 mr-2" fill="currentColor" viewBox="0 0 20 20">
              <path d="M16.707 5.293a1 1 0 010 1.414L8.414 15H6v-2.414l8.293-8.293a1 1 0 011.414 0z"></path>
            </svg>
            <span data-pt="Mais de 150 alunos formados" data-en="Over 100 successful students">Mais de 150 alunos formados</span>
          </li>
          <li class="flex items-center text-purple-100">
            <svg class="w-5 h-5 text-indigo-600 mr-2" fill="currentColor" viewBox="0 0 20 20">
              <path d="M16.707 5.293a1 1 0 010 1.414L8.414 15H6v-2.414l8.293-8.293a1 1 0 011.414 0z"></path>
            </svg>
            <span data-pt="Suporte dedicado" data-en="Dedicated support">Suporte individual para cada aluno</span>
          </li>
          <li class="flex items-center text-purple-100">
            <svg class="w-5 h-5 text-indigo-600 mr-2" fill="currentColor" viewBox="0 0 20 20">
              <path d="M16.707 5.293a1 1 0 010 1.414L8.414 15H6v-2.414l8.293-8.293a1 1 0 011.414 0z"></path>
            </svg>
            <span data-pt="Acesso vitalício às aulas" data-en="Lifetime access to course">Acesso vitalício às aulas</span>
          </li>
          <li class="flex items-center text-purple-100">
            <svg class="w-5 h-5 text-indigo-600 mr-2" fill="currentColor" viewBox="0 0 20 20">
              <path d="M16.707 5.293a1 1 0 010 1.414L8.414 15H6v-2.414l8.293-8.293a1 1 0 011.414 0z"></path>
            </svg>
            <span data-pt="Aprenda usar somente as ferramentas essenciais" data-en="Learn to use only the essential tools">Aprenda usar somente as ferramentas essenciais</span>
          </li>
        </ul>
        <a href="https://discord.gg/kBAHaNbqYH" 
        class="block bg-purple-800 text-white py-2 rounded-lg hover:bg-purple-900 text-center" 
        data-href-pt="https://discord.gg/kBAHaNbqYH" 
        data-pt="Comprar Agora" 
        data-en="Buy Now" 
        data-href-en="https://discord.gg/kBAHaNbqYH">Comprar Agora</a>
      </div>
    </div>
  
          <!-- Enterprise Plan -->
          <div class="bg-gray-900 bg-opacity-40 rounded-lg shadow-lg p-6">
            <h3 class="text-lg font-extrabold text-purple-700 mb-4 text-center">Métodos Anti-Bypass 🐱‍👤</h3>
            <p class="text-purple-300 mb-6 text-center">Pra você nunca mais tomar bypass na sua vida e fazer exposed. 😝😎</p>
            <div class="text-4xl font-extrabold text-purple-700 mb-4 text-center">R$ 120,00<span class="text-lg text-purple-300 font-medium">/lifetime</span></div>
            <ul class="mb-6 space-y-2">
              <li class="flex items-center text-purple-100">
                <svg class="w-5 h-5 text-indigo-600 mr-2" fill="currentColor" viewBox="0 0 20 20">
                  <path d="M16.707 5.293a1 1 0 010 1.414L8.414 15H6v-2.414l8.293-8.293a1 1 0 011.414 0z"></path>
                </svg>
                <span data-pt="Métodos específicos para todos os bypass do mercado" data-en="Specific methods for all bypasses on the market">Métodos específicos para todos os bypass do mercado</span>
              </li>
              <li class="flex items-center text-purple-100">
                <svg class="w-5 h-5 text-indigo-600 mr-2" fill="currentColor" viewBox="0 0 20 20">
                  <path d="M16.707 5.293a1 1 0 010 1.414L8.414 15H6v-2.414l8.293-8.293a1 1 0 011.414 0z"></path>
                </svg>
                <span data-pt="Ferramentas únicas e novos métodos de detecção" data-en="Unique tools and new detection methods">Ferramentas únicas e novos métodos de detecção</span>
              </li>
              <li class="flex items-center text-purple-100">
                <svg class="w-5 h-5 text-indigo-600 mr-2" fill="currentColor" viewBox="0 0 20 20">
                  <path d="M16.707 5.293a1 1 0 010 1.414L8.414 15H6v-2.414l8.293-8.293a1 1 0 011.414 0z"></path>
                </svg>
                <span data-pt="Comunidade ativa de teladores experientes para trocar conhecimento" data-en="Active community of experienced screeners to exchange knowledge">Comunidade ativa de teladores experientes</span>
              </li>
              <li class="flex items-center text-purple-100">
                <svg class="w-5 h-5 text-indigo-600 mr-2" fill="currentColor" viewBox="0 0 20 20">
                  <path d="M16.707 5.293a1 1 0 010 1.414L8.414 15H6v-2.414l8.293-8.293a1 1 0 011.414 0z"></path>
                </svg>
                Webinars gratuitamente exclusivos com os professores mensalmente
              </li>
              <li class="flex items-center text-purple-100">
                <svg class="w-5 h-5 text-indigo-600 mr-2" fill="currentColor" viewBox="0 0 20 20">
                  <path d="M16.707 5.293a1 1 0 010 1.414L8.414 15H6v-2.414l8.293-8.293a1 1 0 011.414 0z"></path>
                </svg>
                <span data-pt="Acesso vitalício aos métodos constatemente atualizados" data-en="Lifetime access to constantly updated methods">Acesso vitalício aos métodos constatemente atualizados</span>
              </li>
            </ul>
            <a href="https://discord.gg/kBAHaNbqYH" 
            class="block bg-purple-800 text-white py-2 rounded-lg hover:bg-purple-900 text-center" 
            data-href-pt="https://discord.gg/kBAHaNbqYH" 
            data-pt="Comprar Agora" 
            data-en="Not Available Yet" 
            data-href-en="https://discord.gg/kBAHaNbqYH">Comprar Agora</a>
          </div>
        </div>
      </div>
    </section>
    
    
    
  
  <section id="partners" class="py-20 bg-black relative" data-aos="fade-up" data-aos-duration="1800">
    <div class="container mx-auto text-center px-6">
        <!-- Título com tradução -->
        <h3 class="text-3xl font-bold text-purple-500 mb-4" 
            data-pt="Parceiros" 
            data-en="Partners">Parceiros</h3>

        <!-- Parágrafo com tradução separada -->
        <p class="text-gray-400 mb-8">
            <span data-pt="Conheça os parceiros que tornam o" data-en="Meet the partners that make">Conheça os parceiros que tornam o</span>
            <span class="text-purple-400 font-semibold">Ecoss ScreenShare</span>
            <span data-pt="possível." data-en="possible.">possível.</span>
        </p>
</section>
  
  
  
  

    
      <!-- Script para alternar idiomas -->
      <script>
        function switchLanguage(lang) {
            document.querySelectorAll('[data-pt]').forEach((element) => {
                // Alterar o texto com base no idioma
                const text = element.getAttribute(`data-${lang}`);
                if (text) {
                    element.textContent = text;
                }
    
                // Alterar o href com base no idioma
                if (lang === 'en' && element.hasAttribute('data-href-en')) {
                    element.setAttribute('href', element.getAttribute('data-href-en'));
                } else if (lang === 'pt' && element.hasAttribute('data-href-pt')) {
                    element.setAttribute('href', element.getAttribute('data-href-pt'));
                }
            });
        }
    
        // Listeners para os botões de idioma
        document.getElementById('btn-pt').addEventListener('click', () => switchLanguage('pt'));
        document.getElementById('btn-en').addEventListener('click', () => switchLanguage('en'));
    </script>
    

<!-- Footer -->
<footer class="bg-black-900 py-6">
    <div class="container mx-auto text-center text-black-400">
        <p>
            &copy; 2024 <span class="text-purple-400 font-semibold">6siz ScreenShare</span>. 
            <span data-pt="Todos os direitos reservados." data-en="All rights reserved.">Todos os direitos reservados.</span>
        </p>
    </div>
</footer>

<script>
    document.addEventListener('DOMContentLoaded', () => {
        const textToType = "Ecoss ScreenShare"; // Texto que será digitado
        const typingSpeed = 250; // Velocidade de digitação em milissegundos
        const cursorBlinkSpeed = 500; // Velocidade do cursor piscando

        const h1Element = document.getElementById('typing-effect');
        let currentText = "";
        let index = 0;

        // Função para simular digitação
        function typeEffect() {
            if (index < textToType.length) {
                currentText += textToType[index];
                h1Element.textContent = currentText + "|"; // Adiciona o cursor
                index++;
                setTimeout(typeEffect, typingSpeed);
            } else {
                // Remove o cursor após a digitação
                h1Element.textContent = currentText;
            }
        }

        // Função para piscar o cursor
        function startCursorBlink() {
            setInterval(() => {
                if (h1Element.textContent.endsWith("|")) {
                    h1Element.textContent = h1Element.textContent.slice(0, -1); // Remove o cursor
                } else {
                    h1Element.textContent += "|"; // Adiciona o cursor
                }
            }, cursorBlinkSpeed);
        }

        // Inicia o efeito de digitação
        typeEffect();
    });
</script>

</body>
</html>
