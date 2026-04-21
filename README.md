<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SIRC - Notificação de Débito #99283 | Danila Ferreira</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        sirc: {
                            red: '#DC2626',
                            dark: '#1F2937',
                            gray: '#374151',
                            light: '#F3F4F6',
                        }
                    },
                    animation: {
                        'pulse-slow': 'pulse 3s cubic-bezier(0.4, 0, 0.6, 1) infinite',
                        'bounce-slow': 'bounce 2s infinite',
                        'shake': 'shake 0.5s cubic-bezier(.36,.07,.19,.97) both',
                    },
                    keyframes: {
                        shake: {
                            '10%, 90%': { transform: 'translate3d(-1px, 0, 0)' },
                            '20%, 80%': { transform: 'translate3d(2px, 0, 0)' },
                            '30%, 50%, 70%': { transform: 'translate3d(-4px, 0, 0)' },
                            '40%, 60%': { transform: 'translate3d(4px, 0, 0)' }
                        }
                    }
                }
            }
        }
    </script>
    <style>
        .gradient-bg {
            background: linear-gradient(135deg, #DC2626 0%, #991B1B 100%);
        }
        .glass-effect {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        .countdown-box {
            background: linear-gradient(145deg, #1F2937, #111827);
            box-shadow: 0 10px 40px -10px rgba(0,0,0,0.3);
        }
        .danger-border {
            border-left: 4px solid #DC2626;
        }
        .pix-container {
            background: linear-gradient(145deg, #F0FDF4, #DCFCE7);
            border: 2px solid #16A34A;
        }
        .warning-stripes {
            background: repeating-linear-gradient(
                45deg,
                #FEF3C7,
                #FEF3C7 10px,
                #FDE68A 10px,
                #FDE68A 20px
            );
        }
    </style>
</head>
<body class="bg-gray-100 font-sans antialiased">

    <!-- Top Warning Bar -->
    <div class="warning-stripes py-2 px-4 text-center border-b-2 border-yellow-500">
        <p class="text-yellow-900 font-bold text-sm uppercase tracking-wider animate-pulse">
            <i class="fas fa-exclamation-triangle mr-2"></i>
            Notificação Oficial - Prazo Limitado de 2 Meses
        </p>
    </div>

    <!-- Header -->
    <header class="gradient-bg text-white py-8 px-4 shadow-2xl relative overflow-hidden">
        <div class="absolute inset-0 opacity-10">
            <svg class="w-full h-full" viewBox="0 0 100 100" preserveAspectRatio="none">
                <pattern id="grid" width="10" height="10" patternUnits="userSpaceOnUse">
                    <path d="M 10 0 L 0 0 0 10" fill="none" stroke="white" stroke-width="0.5"/>
                </pattern>
                <rect width="100" height="100" fill="url(#grid)"/>
            </svg>
        </div>
        <div class="max-w-4xl mx-auto relative z-10">
            <div class="flex items-center justify-between mb-4">
                <div class="flex items-center space-x-3">
                    <div class="bg-white/20 p-3 rounded-lg backdrop-blur-sm">
                        <i class="fas fa-shield-alt text-2xl"></i>
                    </div>
                    <div>
                        <h1 class="text-2xl font-black tracking-tight">SIRC</h1>
                        <p class="text-red-100 text-xs uppercase tracking-widest">Sistema Integrado de Restrição de Crédito</p>
                    </div>
                </div>
                <div class="text-right hidden sm:block">
                    <p class="text-xs text-red-200">Protocolo</p>
                    <p class="font-mono font-bold text-lg">#99283</p>
                </div>
            </div>
            <div class="mt-6 bg-white/10 backdrop-blur-md rounded-lg p-4 border border-white/20">
                <p class="text-sm text-red-100 mb-1">Destinatário:</p>
                <h2 class="text-xl font-bold">Sra. Danila Ferreira</h2>
                <p class="text-red-200 text-sm mt-1">Notificação de Débito em Aberto</p>
            </div>
        </div>
    </header>

    <main class="max-w-4xl mx-auto px-4 py-8 space-y-6">

        <!-- Alert Banner -->
        <div class="bg-red-50 border-l-4 border-red-600 p-4 rounded-r-lg shadow-sm">
            <div class="flex items-start">
                <i class="fas fa-gavel text-red-600 text-xl mt-1 mr-3"></i>
                <div>
                    <h3 class="text-red-900 font-bold text-lg mb-1">Atenção: Prazo Judicial de 2 Meses</h3>
                    <p class="text-red-800 text-sm leading-relaxed">
                        O débito de <strong>R$ 4.000,00</strong> permanece em aberto. A Sra. tem um prazo de 
                        <strong>2 (dois) meses</strong> para regularizar voluntariamente a pendência. 
                        Após esse prazo, o caso será tratado <strong>EXCLUSIVAMENTE</strong> pela via judicial.
                    </p>
                </div>
            </div>
        </div>

        <!-- Countdown Timer -->
        <div class="countdown-box rounded-2xl p-6 text-white">
            <h3 class="text-center text-gray-400 text-sm uppercase tracking-widest mb-4">
                <i class="fas fa-clock mr-2"></i>Tempo Restante para Regularização
            </h3>
            <div class="grid grid-cols-4 gap-4 max-w-lg mx-auto" id="countdown">
                <div class="text-center">
                    <div class="bg-gray-800 rounded-lg p-3 border border-gray-700">
                        <span class="text-3xl font-black text-red-400" id="days">60</span>
                    </div>
                    <p class="text-xs text-gray-400 mt-1 uppercase">Dias</p>
                </div>
                <div class="text-center">
                    <div class="bg-gray-800 rounded-lg p-3 border border-gray-700">
                        <span class="text-3xl font-black text-red-400" id="hours">00</span>
                    </div>
                    <p class="text-xs text-gray-400 mt-1 uppercase">Horas</p>
                </div>
                <div class="text-center">
                    <div class="bg-gray-800 rounded-lg p-3 border border-gray-700">
                        <span class="text-3xl font-black text-red-400" id="minutes">00</span>
                    </div>
                    <p class="text-xs text-gray-400 mt-1 uppercase">Minutos</p>
                </div>
                <div class="text-center">
                    <div class="bg-gray-800 rounded-lg p-3 border border-gray-700">
                        <span class="text-3xl font-black text-red-400" id="seconds">00</span>
                    </div>
                    <p class="text-xs text-gray-400 mt-1 uppercase">Segundos</p>
                </div>
            </div>
            <div class="mt-4 text-center">
                <p class="text-red-400 text-sm font-semibold animate-pulse">
                    <i class="fas fa-exclamation-circle mr-1"></i>
                    Após o prazo: Protesto + Ação Judicial + Penhora
                </p>
            </div>
        </div>

        <!-- Debt Details -->
        <div class="bg-white rounded-xl shadow-lg overflow-hidden">
            <div class="bg-gray-50 px-6 py-4 border-b border-gray-200 flex items-center justify-between">
                <h3 class="font-bold text-gray-800 flex items-center">
                    <i class="fas fa-file-invoice-dollar mr-2 text-red-600"></i>
                    Detalhes do Débito
                </h3>
                <span class="bg-red-100 text-red-800 text-xs font-bold px-3 py-1 rounded-full">EM ABERTO</span>
            </div>
            <div class="p-6">
                <div class="grid md:grid-cols-2 gap-6">
                    <div class="space-y-4">
                        <div class="flex justify-between items-center py-2 border-b border-gray-100">
                            <span class="text-gray-600 text-sm">Contrato:</span>
                            <span class="font-mono font-bold text-gray-900">99283</span>
                        </div>
                        <div class="flex justify-between items-center py-2 border-b border-gray-100">
                            <span class="text-gray-600 text-sm">Devedor:</span>
                            <span class="font-semibold text-gray-900">Danila Ferreira</span>
                        </div>
                        <div class="flex justify-between items-center py-2 border-b border-gray-100">
                            <span class="text-gray-600 text-sm">Valor Original:</span>
                            <span class="font-semibold text-gray-900">R$ 4.000,00</span>
                        </div>
                        <div class="flex justify-between items-center py-2 border-b border-gray-100">
                            <span class="text-gray-600 text-sm">Status:</span>
                            <span class="text-red-600 font-bold text-sm">PENDENTE</span>
                        </div>
                    </div>
                    <div class="bg-red-50 rounded-lg p-4 border border-red-200">
                        <h4 class="text-red-900 font-bold text-sm mb-3 uppercase tracking-wider">Consequências após o prazo:</h4>
                        <ul class="space-y-2 text-sm text-red-800">
                            <li class="flex items-start">
                                <i class="fas fa-check-circle mt-1 mr-2 text-red-600"></i>
                                <span>Protesto em cartório (Lei 9.492/97)</span>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-check-circle mt-1 mr-2 text-red-600"></i>
                                <span>Inclusão Serasa/SPC (5 anos)</span>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-check-circle mt-1 mr-2 text-red-600"></i>
                                <span>Execução judicial com penhora online</span>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-check-circle mt-1 mr-2 text-red-600"></i>
                                <span>Bloqueio de contas via Sisbajud</span>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-check-circle mt-1 mr-2 text-red-600"></i>
                                <span>Penhora de veículos e imóveis</span>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>

        <!-- PIX Payment Section -->
        <div class="pix-container rounded-2xl p-6 shadow-lg relative overflow-hidden">
            <div class="absolute top-0 right-0 bg-green-600 text-white text-xs font-bold px-4 py-1 rounded-bl-lg">
                RECOMENDADO
            </div>
            <h3 class="text-green-900 font-bold text-xl mb-2 flex items-center">
                <i class="fas fa-qrcode mr-2 text-2xl"></i>
                Pagamento Imediato via PIX
            </h3>
            <p class="text-green-800 text-sm mb-6">
                Regularize sua pendência agora mesmo. O pagamento via PIX é processado em segundos e sua situação será atualizada automaticamente.
            </p>

            <div class="bg-white rounded-xl p-6 shadow-inner max-w-md mx-auto text-center">
                <div id="pix-qr-container" class="mb-4">
                    <div class="bg-gray-100 p-4 rounded-lg inline-block mb-3">
                        <svg id="pix-qr" viewBox="0 0 200 200" class="w-48 h-48 mx-auto"></svg>
                    </div>
                    <p class="text-xs text-gray-500 mb-2">Escaneie o QR Code com seu aplicativo bancário</p>
                </div>

                <div class="space-y-3">
                    <div class="bg-gray-50 rounded-lg p-3 border border-gray-200">
                        <p class="text-xs text-gray-500 uppercase tracking-wider mb-1">Chave PIX (Copia e Cola)</p>
                        <div class="flex items-center gap-2">
                            <input type="text" id="pix-code" readonly 
                                class="flex-1 bg-white border border-gray-300 rounded px-3 py-2 text-xs font-mono text-gray-700 focus:outline-none focus:ring-2 focus:ring-green-500"
                                value="">
                            <button onclick="copyPix()" 
                                class="bg-green-600 hover:bg-green-700 text-white px-4 py-2 rounded-lg text-sm font-semibold transition-colors flex items-center gap-2">
                                <i class="fas fa-copy"></i>
                                Copiar
                            </button>
                        </div>
                    </div>

                    <button onclick="generateNewPix()" 
                        class="w-full bg-green-600 hover:bg-green-700 text-white font-bold py-3 px-6 rounded-lg shadow-lg hover:shadow-xl transition-all transform hover:-translate-y-0.5 flex items-center justify-center gap-2">
                        <i class="fas fa-sync-alt"></i>
                        Gerar Novo Código PIX
                    </button>

                    <p class="text-xs text-green-700 mt-2">
                        <i class="fas fa-lock mr-1"></i>
                        Pagamento seguro processado em ambiente criptografado
                    </p>
                </div>
            </div>
        </div>

        <!-- Warning Section -->
        <div class="bg-gray-900 text-white rounded-xl p-6 shadow-xl">
            <h3 class="text-xl font-bold mb-4 flex items-center text-red-400">
                <i class="fas fa-user-secret mr-2"></i>
                "NÃO ADIANTA SE ESCONDER"
            </h3>
            <div class="grid md:grid-cols-2 gap-4">
                <div class="space-y-3">
                    <div class="flex items-start space-x-3 bg-gray-800 p-3 rounded-lg">
                        <i class="fas fa-phone-slash text-red-400 mt-1"></i>
                        <div>
                            <p class="font-semibold text-sm">Mudar de número?</p>
                            <p class="text-gray-400 text-xs">O sistema localiza automaticamente.</p>
                        </div>
                    </div>
                    <div class="flex items-start space-x-3 bg-gray-800 p-3 rounded-lg">
                        <i class="fas fa-home text-red-400 mt-1"></i>
                        <div>
                            <p class="font-semibold text-sm">Trocar de endereço?</p>
                            <p class="text-gray-400 text-xs">Citação por edital ou oficial de justiça.</p>
                        </div>
                    </div>
                </div>
                <div class="space-y-3">
                    <div class="flex items-start space-x-3 bg-gray-800 p-3 rounded-lg">
                        <i class="fas fa-university text-red-400 mt-1"></i>
                        <div>
                            <p class="font-semibold text-sm">Fechar contas bancárias?</p>
                            <p class="text-gray-400 text-xs">Novas contas também serão bloqueadas via SCB.</p>
                        </div>
                    </div>
                    <div class="flex items-start space-x-3 bg-gray-800 p-3 rounded-lg">
                        <i class="fas fa-eye-slash text-red-400 mt-1"></i>
                        <div>
                            <p class="font-semibold text-sm">"Não vi a notificação"?</p>
                            <p class="text-gray-400 text-xs">Notificação válida e registrada no sistema.</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="mt-4 p-3 bg-red-900/30 border border-red-800 rounded-lg text-center">
                <p class="text-red-300 text-sm font-semibold">
                    A única saída é regularizar ou negociar dentro de 2 meses.
                </p>
            </div>
        </div>

        <!-- Contact Section -->
        <div class="bg-white rounded-xl shadow-lg p-6">
            <h3 class="font-bold text-gray-800 mb-4 flex items-center">
                <i class="fas fa-headset mr-2 text-blue-600"></i>
                Central de Atendimento SIRC
            </h3>
            <div class="flex flex-col sm:flex-row items-center justify-between gap-4">
                <div class="flex items-center space-x-4">
                    <div class="bg-blue-100 p-3 rounded-full">
                        <i class="fas fa-phone-alt text-blue-600 text-xl"></i>
                    </div>
                    <div>
                        <p class="text-xs text-gray-500 uppercase">Telefone/WhatsApp</p>
                        <a href="tel:+55889865439707" class="text-xl font-bold text-gray-900 hover:text-blue-600 transition-colors">
                            (88) 98654-39707
                        </a>
                    </div>
                </div>
                <div class="flex gap-3">
                    <button onclick="window.print()" class="bg-gray-100 hover:bg-gray-200 text-gray-700 px-4 py-2 rounded-lg text-sm font-semibold transition-colors flex items-center gap-2">
                        <i class="fas fa-print"></i>
                        Imprimir
                    </button>
                    <a href="https://wa.me/55889865439707" target="_blank" 
                        class="bg-green-500 hover:bg-green-600 text-white px-6 py-2 rounded-lg text-sm font-bold transition-colors flex items-center gap-2 shadow-lg">
                        <i class="fab fa-whatsapp"></i>
                        Falar no WhatsApp
                    </a>
                </div>
            </div>
        </div>

        <!-- Legal Footer -->
        <div class="text-center text-gray-500 text-xs space-y-2 pb-8">
            <p>SIRC - Sistema Integrado de Restrição de Crédito</p>
            <p>Documento gerado em: <span id="current-date"></span></p>
            <p class="text-gray-400">Esta notificação é válida e registrada conforme Lei 9.492/97</p>
        </div>

    </main>

    <!-- Copy Toast -->
    <div id="toast" class="fixed bottom-4 right-4 bg-green-600 text-white px-6 py-3 rounded-lg shadow-2xl transform translate-y-20 transition-transform duration-300 flex items-center gap-2 z-50">
        <i class="fas fa-check-circle"></i>
        <span class="font-semibold">Código PIX copiado!</span>
    </div>

    <script>
        // Countdown Timer
        const targetDate = new Date();
        targetDate.setDate(targetDate.getDate() + 60); // 2 months approx

        function updateCountdown() {
            const now = new Date();
            const diff = targetDate - now;

            if (diff <= 0) {
                document.getElementById('days').textContent = '00';
                document.getElementById('hours').textContent = '00';
                document.getElementById('minutes').textContent = '00';
                document.getElementById('seconds').textContent = '00';
                return;
            }

            const days = Math.floor(diff / (1000 * 60 * 60 * 24));
            const hours = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((diff % (1000 * 60)) / 1000);

            document.getElementById('days').textContent = String(days).padStart(2, '0');
            document.getElementById('hours').textContent = String(hours).padStart(2, '0');
            document.getElementById('minutes').textContent = String(minutes).padStart(2, '0');
            document.getElementById('seconds').textContent = String(seconds).padStart(2, '0');
        }

        setInterval(updateCountdown, 1000);
        updateCountdown();

        // Current Date
        document.getElementById('current-date').textContent = new Date().toLocaleDateString('pt-BR', {
            day: '2-digit',
            month: '2-digit',
            year: 'numeric',
            hour: '2-digit',
            minute: '2-digit'
        });

        // PIX QR Code Generator (Simulated)
        function generateQRCode(text) {
            const svg = document.getElementById('pix-qr');
            svg.innerHTML = '';
            
            // Create a simulated QR code pattern
            const size = 25;
            const cellSize = 200 / size;
            
            // Background
            const rect = document.createElementNS('http://www.w3.org/2000/svg', 'rect');
            rect.setAttribute('width', '200');
            rect.setAttribute('height', '200');
            rect.setAttribute('fill', 'white');
            svg.appendChild(rect);
            
            // Generate pseudo-random pattern based on text
            let seed = 0;
            for (let i = 0; i < text.length; i++) {
                seed += text.charCodeAt(i);
            }
            
            const random = () => {
                const x = Math.sin(seed++) * 10000;
                return x - Math.floor(x);
            };
            
            // Corner markers (position detection patterns)
            const markers = [
                {x: 2, y: 2}, {x: size-5, y: 2}, {x: 2, y: size-5}
            ];
            
            markers.forEach(m => {
                // Outer square
                const outer = document.createElementNS('http://www.w3.org/2000/svg', 'rect');
                outer.setAttribute('x', m.x * cellSize);
                outer.setAttribute('y', m.y * cellSize);
                outer.setAttribute('width', 7 * cellSize);
                outer.setAttribute('height', 7 * cellSize);
                outer.setAttribute('fill', '#000033');
                svg.appendChild(outer);
                
                // Inner white
                const inner = document.createElementNS('http://www.w3.org/2000/svg', 'rect');
                inner.setAttribute('x', (m.x + 1) * cellSize);
                inner.setAttribute('y', (m.y + 1) * cellSize);
                inner.setAttribute('width', 5 * cellSize);
                inner.setAttribute('height', 5 * cellSize);
                inner.setAttribute('fill', 'white');
                svg.appendChild(inner);
                
                // Center black
                const center = document.createElementNS('http://www.w3.org/2000/svg', 'rect');
                center.setAttribute('x', (m.x + 2) * cellSize);
                center.setAttribute('y', (m.y + 2) * cellSize);
                center.setAttribute('width', 3 * cellSize);
                center.setAttribute('height', 3 * cellSize);
                center.setAttribute('fill', '#000033');
                svg.appendChild(center);
            });
            
            // Data modules
            for (let i = 0; i < size; i++) {
                for (let j = 0; j < size; j++) {
                    // Skip position detection patterns
                    if ((i < 9 && j < 9) || (i > size-10 && j < 9) || (i < 9 && j > size-10)) continue;
                    
                    if (random() > 0.5) {
                        const module = document.createElementNS('http://www.w3.org/2000/svg', 'rect');
                        module.setAttribute('x', i * cellSize);
                        module.setAttribute('y', j * cellSize);
                        module.setAttribute('width', cellSize);
                        module.setAttribute('height', cellSize);
                        module.setAttribute('fill', '#000033');
                        svg.appendChild(module);
                    }
                }
            }
        }

        function generatePixPayload() {
            // Simulated PIX payload format
            const id = Math.random().toString(36).substring(2, 15).toUpperCase();
            const payload = `00020126440014BR.GOV.PIX0111SIRC-CREDITO52040000530398654064000.005802BR5922SIRC SISTEMA RESTRICAO6009SAO PAULO62290525CONTRATO99283DANILA${id}6304`;
            
            // Calculate CRC16
            let crc = 0xFFFF;
            for (let i = 0; i < payload.length; i++) {
                crc ^= payload.charCodeAt(i) << 8;
                for (let j = 0; j < 8; j++) {
                    crc = (crc & 0x8000) ? (crc << 1) ^ 0x1021 : crc << 1;
                }
            }
            crc &= 0xFFFF;
            const crcStr = crc.toString(16).toUpperCase().padStart(4, '0');
            
            return payload + crcStr;
        }

        function generateNewPix() {
            const payload = generatePixPayload();
            document.getElementById('pix-code').value = payload;
            generateQRCode(payload);
            
            // Visual feedback
            const btn = document.querySelector('button[onclick="generateNewPix()"]');
            const originalHTML = btn.innerHTML;
            btn.innerHTML = '<i class="fas fa-check"></i> Código Gerado!';
            btn.classList.add('bg-green-700');
            setTimeout(() => {
                btn.innerHTML = originalHTML;
                btn.classList.remove('bg-green-700');
            }, 2000);
        }

        function copyPix() {
            const input = document.getElementById('pix-code');
            input.select();
            input.setSelectionRange(0, 99999);
            navigator.clipboard.writeText(input.value).then(() => {
                const toast = document.getElementById('toast');
                toast.classList.remove('translate-y-20');
                setTimeout(() => {
                    toast.classList.add('translate-y-20');
                }, 3000);
            });
        }

        // Initialize
        generateNewPix();

        // Shake animation on load for urgency
        setTimeout(() => {
            document.querySelector('.countdown-box').classList.add('animate-shake');
            setTimeout(() => {
                document.querySelector('.countdown-box').classList.remove('animate-shake');
            }, 500);
        }, 1000);
    </script>
</body>
</html>
