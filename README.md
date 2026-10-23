<html lang="zh-CN" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IYKYK TICKET | 韩国本土预售票务管家</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Noto+Sans+KR:wght@300;400;500;700&display=swap" rel="stylesheet">
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        kpink: {
                            50: '#FFF5F7',   // Softest Pastel Pink
                            100: '#FFE3E8',  // Light blush
                            200: '#FFD6E0',  // Pastel Pink border/accent
                            300: '#FFB3C6',  // Medium Rose
                            400: '#FF85A1',  // Primary Accent Pink
                            500: '#FF5C8A',  // Deep Rose Accent
                            600: '#E03A6E',
                        },
                        ktext: {
                            primary: '#2D3748',   // Charcoal Slate
                            secondary: '#718096', // Neutral Cool Gray
                            light: '#A0AEC0'
                        },
                        kbg: '#FCF8F9'
                    },
                    fontFamily: {
                        sans: ['Inter', 'Noto Sans KR', 'sans-serif'],
                    },
                    borderRadius: {
                        '3xl': '1.75rem',
                        '4xl': '2.25rem',
                        '5xl': '2.75rem'
                    },
                    boxShadow: {
                        'soft': '0 12px 32px -8px rgba(255, 179, 198, 0.25)',
                        'soft-lg': '0 20px 48px -12px rgba(255, 133, 161, 0.28)',
                        'card': '0 8px 30px -6px rgba(113, 128, 150, 0.06)'
                    }
                }
            }
        }
    </script>
    <style>
        body {
            background-color: #FCF8F9;
            color: #2D3748;
            font-family: 'Inter', 'Noto Sans KR', sans-serif;
            overflow-x: hidden;
        }

        @keyframes floatSlow {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-6px) rotate(1deg); }
        }

        @keyframes pulseGlow {
            0%, 100% { opacity: 0.35; transform: scale(1); }
            50% { opacity: 0.6; transform: scale(1.05); }
        }

        .animate-float-slow {
            animation: floatSlow 6s ease-in-out infinite;
        }

        .animate-glow {
            animation: pulseGlow 7s ease-in-out infinite;
        }

        .k-glass {
            background: rgba(255, 255, 255, 0.92);
            backdrop-filter: blur(16px);
            -webkit-backdrop-filter: blur(16px);
            border: 1px solid rgba(255, 214, 224, 0.7);
        }

        .no-scrollbar::-webkit-scrollbar {
            display: none;
        }
        .no-scrollbar {
            -ms-overflow-style: none;
            scrollbar-width: none;
        }
    </style>
</head>
<body class="min-h-screen flex flex-col relative selection:bg-kpink-200 selection:text-kpink-600">

    <!-- SUBTLE BACKGROUND DECORATIONS (SOFT KOREAN AESTHETIC - NO TOP SPARKLE/STAR STICKER) -->
    <div class="absolute inset-0 pointer-events-none z-0 overflow-hidden">
        <div class="absolute -top-24 -left-20 w-[32rem] h-[32rem] bg-kpink-100/70 rounded-full blur-3xl opacity-70 animate-glow"></div>
        <div class="absolute top-1/3 -right-24 w-[28rem] h-[28rem] bg-kpink-200/50 rounded-full blur-3xl opacity-50 animate-glow" style="animation-delay: 2.5s;"></div>
        <div class="absolute bottom-1/4 left-1/6 w-[30rem] h-[30rem] bg-rose-100/60 rounded-full blur-3xl opacity-60 animate-glow" style="animation-delay: 4.5s;"></div>
        <div class="absolute inset-0 opacity-[0.02]" style="background-image: radial-gradient(#2D3748 1px, transparent 1px); background-size: 28px 28px;"></div>
    </div>

    <!-- MAIN HEADER -->
    <header class="w-full max-w-6xl mx-auto px-4 sm:px-8 pt-6 pb-2 z-10 relative">
        <div class="k-glass rounded-full px-6 py-3.5 flex items-center justify-between shadow-card">
            <a href="#" class="flex items-center gap-3 group">
                <div class="w-10 h-10 rounded-full bg-gradient-to-tr from-kpink-400 via-kpink-300 to-kpink-200 flex items-center justify-center text-white font-bold text-sm shadow-sm group-hover:scale-105 transition-transform">
                    IY
                </div>
                <div class="flex flex-col">
                    <span class="font-bold tracking-tight text-lg text-ktext-primary flex items-center gap-1.5">
                        IYKYK <span class="text-[10px] font-normal px-2 py-0.5 rounded-full bg-kpink-50 text-kpink-600 border border-kpink-200">Ticket</span>
                    </span>
                </div>
            </a>

            <nav class="hidden md:flex items-center gap-7 text-xs sm:text-sm font-medium text-ktext-secondary">
                <a href="#services" class="hover:text-kpink-500 transition-colors">服务优势</a>
                <a href="#concerts" class="hover:text-kpink-500 transition-colors">演出 Schedule</a>
                <a href="#calculator" class="hover:text-kpink-500 transition-colors">试算测算</a>
                <a href="#orders" class="hover:text-kpink-500 transition-colors">订单查询</a>
                <a href="#trust" class="hover:text-kpink-500 transition-colors">安全保障</a>
            </nav>

            <div class="flex items-center gap-3">
                <button onclick="scrollToSection('orders')" class="hidden sm:flex items-center gap-1.5 bg-white border border-kpink-200 hover:bg-kpink-50 text-ktext-primary font-medium text-xs px-4 py-2 rounded-full transition-all">
                    <i data-lucide="search" class="w-3.5 h-3.5 text-kpink-500"></i>
                    <span>查询订单</span>
                </button>
                <button onclick="scrollToSection('concerts')" class="bg-gradient-to-r from-kpink-400 to-kpink-500 hover:from-kpink-500 hover:to-kpink-600 text-white font-medium text-xs sm:text-sm px-5 py-2 rounded-full shadow-soft hover:shadow-soft-lg transition-all transform hover:-translate-y-0.5">
                    立即预订
                </button>
            </div>
        </div>
    </header>

    <!-- MAIN CONTENT -->
    <main class="flex-grow z-10 max-w-6xl mx-auto px-4 sm:px-6 py-8 space-y-20">

        <!-- HERO SECTION -->
        <section class="relative pt-8 pb-6 text-center flex flex-col items-center justify-center">
            
            <div class="inline-flex items-center gap-2 px-4 py-1.5 rounded-full bg-white/90 border border-kpink-200 text-xs font-medium text-kpink-600 shadow-sm mb-6 animate-float-slow">
                <span class="w-2 h-2 rounded-full bg-kpink-400 animate-ping"></span>
                IYKYK / 韩国本土预售优先抢订服务
            </div>

            <!-- HERO HEADINGS (EXACT REQ) -->
            <h1 class="text-3xl sm:text-5xl md:text-6xl font-bold tracking-tight text-ktext-primary max-w-3xl leading-tight sm:leading-tight mb-4">
                直通韩国本土优先预售通道
            </h1>
            <h2 class="text-2xl sm:text-4xl md:text-5xl font-bold tracking-tight bg-clip-text text-transparent bg-gradient-to-r from-kpink-500 via-kpink-400 to-rose-400 max-w-3xl leading-tight sm:leading-tight mb-6">
                安全·透明·极速抢占优质席位
            </h2>

            <p class="text-xs sm:text-sm md:text-base text-ktext-secondary max-w-2xl font-light leading-relaxed mb-8">
                由专业团队提供<span class="font-medium text-ktext-primary">韩国本土实名认证账号</span>与<span class="font-medium text-ktext-primary">优先开售抢订</span>支持。绕过 Global 通道漫长等候与天价黄牛，采用<span class="text-kpink-600 font-medium">“抢到后付服务费 / 未成功定金全退”</span>安全保障机制。
            </p>

            <!-- Value Highlights -->
            <div class="grid grid-cols-2 sm:grid-cols-4 gap-3 sm:gap-4 w-full max-w-3xl mb-10">
                <div class="k-glass p-4 rounded-3xl text-center shadow-card hover:border-kpink-300 transition-all">
                    <div class="w-8 h-8 mx-auto mb-2 rounded-full bg-kpink-50 flex items-center justify-center text-kpink-500">
                        <i data-lucide="shield-check" class="w-4 h-4"></i>
                    </div>
                    <div class="text-xs font-semibold text-ktext-primary">成功后再付尾款</div>
                    <div class="text-[11px] text-ktext-light mt-0.5">第三方托管低风险</div>
                </div>
                <div class="k-glass p-4 rounded-3xl text-center shadow-card hover:border-kpink-300 transition-all">
                    <div class="w-8 h-8 mx-auto mb-2 rounded-full bg-kpink-50 flex items-center justify-center text-kpink-500">
                        <i data-lucide="zap" class="w-4 h-4"></i>
                    </div>
                    <div class="text-xs font-semibold text-ktext-primary">本土提前优先购票</div>
                    <div class="text-[11px] text-ktext-light mt-0.5">优先抢占内场与VIP</div>
                </div>
                <div class="k-glass p-4 rounded-3xl text-center shadow-card hover:border-kpink-300 transition-all">
                    <div class="w-8 h-8 mx-auto mb-2 rounded-full bg-kpink-50 flex items-center justify-center text-kpink-500">
                        <i data-lucide="user-check" class="w-4 h-4"></i>
                    </div>
                    <div class="text-xs font-semibold text-ktext-primary">在韩实名认证账号</div>
                    <div class="text-[11px] text-ktext-light mt-0.5">避开海外 IP 排队限制</div>
                </div>
                <div class="k-glass p-4 rounded-3xl text-center shadow-card hover:border-kpink-300 transition-all">
                    <div class="w-8 h-8 mx-auto mb-2 rounded-full bg-kpink-50 flex items-center justify-center text-kpink-500">
                        <i data-lucide="sparkles" class="w-4 h-4"></i>
                    </div>
                    <div class="text-xs font-semibold text-ktext-primary">费用明细公开透明</div>
                    <div class="text-[11px] text-ktext-light mt-0.5">服务费 30%-50% 起</div>
                </div>
            </div>

            <!-- Active Status Line -->
            <div class="bg-white/90 border border-kpink-200 shadow-soft rounded-full px-5 py-2.5 flex items-center gap-3 text-xs text-ktext-secondary">
                <span class="flex h-2.5 w-2.5 relative">
                  <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-emerald-400 opacity-75"></span>
                  <span class="relative inline-flex rounded-full h-2.5 w-2.5 bg-emerald-500"></span>
                </span>
                <span>当前本土预售通道运行中：<strong class="text-ktext-primary font-semibold">NCT WISH / aespa / GISELLE / CHANYEOL</strong> 等演出接单中</span>
            </div>
        </section>

        <!-- SECTION 1: CONCERT SCHEDULE & BOOKING HUB -->
        <section id="concerts" class="space-y-6">
            <div class="flex flex-col sm:flex-row sm:items-end justify-between gap-4">
                <div>
                    <div class="text-xs font-semibold text-kpink-500 uppercase tracking-wider mb-1 flex items-center gap-1">
                        Live Concert Schedule
                    </div>
                    <h2 class="text-2xl sm:text-3xl font-bold text-ktext-primary">热门演出与代抢预订列表</h2>
                    <p class="text-xs sm:text-sm text-ktext-secondary mt-1">
                        同步韩国本土 (KR Page) 与全球 (Global Page) 官方预售节点
                    </p>
                </div>
                
                <!-- Search & Category Filter (search box centered) -->
                <div class="flex flex-wrap items-center justify-center gap-2 w-full sm:w-auto">
                    <div class="relative mx-auto sm:mx-0">
                        <i data-lucide="search" class="w-3.5 h-3.5 text-ktext-light absolute left-3 top-1/2 -translate-y-1/2"></i>
                        <input type="text" id="concert-search" oninput="filterConcerts()" placeholder="搜索艺人/场地..." class="bg-white/90 border border-kpink-200 rounded-full pl-9 pr-4 py-1.5 text-xs text-ktext-primary focus:outline-none focus:ring-2 focus:ring-kpink-300">
                    </div>

                    <div class="flex items-center gap-1.5 bg-white/80 p-1 rounded-full border border-kpink-100 text-xs font-medium">
                        <button onclick="setCategoryFilter('all')" id="tab-all" class="concert-tab bg-kpink-400 text-white px-3.5 py-1 rounded-full transition-all shadow-sm">全部</button>
                        <button onclick="setCategoryFilter('dome')" id="tab-dome" class="concert-tab text-ktext-secondary hover:text-ktext-primary px-3.5 py-1 rounded-full transition-all">大型/Dome</button>
                        <button onclick="setCategoryFilter('fanmeeting')" id="tab-fanmeeting" class="concert-tab text-ktext-secondary hover:text-ktext-primary px-3.5 py-1 rounded-full transition-all">FM/Party</button>
                    </div>
                </div>
            </div>

            <div id="concert-grid" class="grid grid-cols-1 md:grid-cols-2 gap-6">
                <!-- Injected via JS -->
            </div>
        </section>

        <!-- SECTION 2: SERVICE PLANS -->
        <section id="services" class="space-y-6">
            <div class="text-center space-y-2 max-w-xl mx-auto">
                <span class="text-xs font-semibold text-kpink-500 uppercase tracking-wider">Transparent Service Plans</span>
                <h2 class="text-2xl sm:text-3xl font-bold text-ktext-primary">选择最适合您的代抢服务方案</h2>
                <p class="text-xs sm:text-sm text-ktext-secondary">
                    包含本土实名认证账号使用权、抢订操作及全程票务对接指导
                </p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                <!-- Plan A -->
                <div class="k-glass rounded-4xl p-6 sm:p-8 border-2 border-kpink-300 relative shadow-soft flex flex-col justify-between space-y-6">
                    <div class="absolute -top-3.5 right-6 bg-gradient-to-r from-kpink-400 to-kpink-500 text-white text-xs font-medium px-4 py-1 rounded-full shadow-sm">
                        推荐 · 92% 用户首选
                    </div>
                    <div class="space-y-4">
                        <div class="w-10 h-10 rounded-2xl bg-kpink-100 flex items-center justify-center text-kpink-600">
                            <i data-lucide="shield-check" class="w-5 h-5"></i>
                        </div>
                        <div>
                            <h3 class="text-lg font-bold text-ktext-primary">抢到后付模式 (Success-First)</h3>
                            <p class="text-xs text-ktext-secondary mt-1">资金安全优先，出票成功后再付主体服务费</p>
                        </div>
                        <div class="text-2xl font-bold text-kpink-600">
                            小额定金 ¥150 <span class="text-xs font-normal text-ktext-secondary">+ 成功后补清服务费 (30%~50%)</span>
                        </div>
                        <ul class="text-xs text-ktext-secondary space-y-2.5 pt-2">
                            <li class="flex items-center gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-emerald-500 shrink-0"></i>
                                <span>分配专人韩国本土实名认证账号</span>
                            </li>
                            <li class="flex items-center gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-emerald-500 shrink-0"></i>
                                <span>抢票未成功：定金 100% 退还或免费转咨询指导</span>
                            </li>
                            <li class="flex items-center gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-emerald-500 shrink-0"></i>
                                <span>成功出票后才付清尾款，支持第三方担保托管</span>
                            </li>
                        </ul>
                    </div>
                    <button onclick="openBookingModal('Success-First')" class="w-full bg-gradient-to-r from-kpink-400 to-kpink-500 hover:from-kpink-500 hover:to-kpink-600 text-white font-medium py-3 rounded-full text-xs shadow-soft transition-all">
                        按此方案预订
                    </button>
                </div>

                <!-- Plan B -->
                <div class="k-glass rounded-4xl p-6 sm:p-8 border border-kpink-200 relative shadow-card flex flex-col justify-between space-y-6">
                    <div class="space-y-4">
                        <div class="w-10 h-10 rounded-2xl bg-kpink-100 flex items-center justify-center text-kpink-600">
                            <i data-lucide="award" class="w-5 h-5"></i>
                        </div>
                        <div>
                            <h3 class="text-lg font-bold text-ktext-primary">VIP 前排锁位方案 (VIP Priority)</h3>
                            <p class="text-xs text-ktext-secondary mt-1">适合拟冲刺首尔内场 VIP / 极其紧缺席位</p>
                        </div>
                        <div class="text-2xl font-bold text-ktext-primary">
                            预付定金 ¥300 <span class="text-xs font-normal text-ktext-secondary">+ 优先队列极速响应</span>
                        </div>
                        <ul class="text-xs text-ktext-secondary space-y-2.5 pt-2">
                            <li class="flex items-center gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-emerald-500 shrink-0"></i>
                                <span>优先调配高响应度本土账号组</span>
                            </li>
                            <li class="flex items-center gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-emerald-500 shrink-0"></i>
                                <span>专属客服一对一全程同步抢票截图</span>
                            </li>
                            <li class="flex items-center gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-emerald-500 shrink-0"></i>
                                <span>未出票全额无损退款，零扣费风险</span>
                            </li>
                        </ul>
                    </div>
                    <button onclick="openBookingModal('VIP-Priority')" class="w-full bg-white hover:bg-kpink-50 border border-kpink-200 text-ktext-primary font-medium py-3 rounded-full text-xs transition-all">
                        按此方案预订
                    </button>
                </div>
            </div>
        </section>

        <!-- SECTION 3: TRANSPARENT CALCULATOR -->
        <section id="calculator" class="k-glass rounded-4xl p-6 sm:p-10 shadow-soft border border-kpink-200">
            <div class="max-w-3xl mx-auto space-y-8">
                <div class="text-center space-y-2">
                    <span class="text-xs font-semibold text-kpink-500 uppercase tracking-wider">Cost Transparency</span>
                    <h2 class="text-2xl sm:text-3xl font-bold text-ktext-primary">代抢服务费用实时测算</h2>
                    <p class="text-xs sm:text-sm text-ktext-secondary max-w-xl mx-auto">
                        拒绝黄牛动辄数倍的恶劣溢价。依据官方票面与合理服务费率计算，拒绝隐藏收费。
                    </p>
                </div>

                <div class="bg-white/90 rounded-3xl p-6 sm:p-8 border border-kpink-100 shadow-sm space-y-6">
                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
                        <div class="space-y-2">
                            <label class="block text-xs font-semibold text-ktext-primary">选择拟代抢演出项目</label>
                            <select id="calc-show" onchange="updateCalculator()" class="w-full bg-kbg border border-kpink-200 rounded-2xl px-4 py-3 text-xs sm:text-sm text-ktext-primary focus:outline-none focus:ring-2 focus:ring-kpink-300">
                                <option value="165000">NCT WISH (一般席) - 165,000 韩元</option>
                                <option value="220000">NCT WISH (VIP席) - 220,000 韩元</option>
                                <option value="121000" selected>aespa FAN MEETING - 121,000 韩元</option>
                                <option value="77000">GISELLE / CHANYEOL 生日会 - 77,000 韩元</option>
                                <option value="143000">AND2BLE FAN-CON - 143,000 韩元</option>
                                <option value="154000">NMIXX 1ST WORLD TOUR - 154,000 韩元</option>
                            </select>
                        </div>

                        <div class="space-y-2">
                            <label class="block text-xs font-semibold text-ktext-primary">服务档位</label>
                            <select id="calc-markup" onchange="updateCalculator()" class="w-full bg-kbg border border-kpink-200 rounded-2xl px-4 py-3 text-xs sm:text-sm text-ktext-primary focus:outline-none focus:ring-2 focus:ring-kpink-300">
                                <option value="0.30">基础档: 30% 服务费 (一般席位/看台)</option>
                                <option value="0.50" selected>标准档: 50% 服务费 (热门推荐)</option>
                                <option value="0.70">冲刺档: 70% 服务费 (稀缺前排 VIP)</option>
                            </select>
                        </div>
                    </div>

                    <div class="pt-4 border-t border-kpink-100">
                        <div class="grid grid-cols-1 md:grid-cols-3 gap-4 text-center">
                            <div class="p-4 rounded-2xl bg-gray-50 border border-gray-100 space-y-1">
                                <div class="text-xs font-bold text-gray-500">官方原票价 (折合RMB)</div>
                                <div class="text-lg font-bold text-gray-700" id="calc-cost-face">¥ 638</div>
                                <div class="text-[10px] text-gray-400">按实时汇率折算</div>
                            </div>

                            <div class="p-4 rounded-2xl bg-kpink-50 border-2 border-kpink-300 space-y-1 relative shadow-sm">
                                <div class="text-xs font-bold text-kpink-600">IYKYK 预估总支出</div>
                                <div class="text-xl font-extrabold text-kpink-600" id="calc-cost-iykyk">¥ 957</div>
                                <div class="text-[10px] text-kpink-500 font-medium" id="calc-fee-detail">含服务费 ¥319</div>
                            </div>

                            <div class="p-4 rounded-2xl bg-rose-50/60 border border-rose-100 space-y-1">
                                <div class="text-xs font-bold text-rose-500">传统二手黄牛参考价</div>
                                <div class="text-lg font-bold text-rose-600" id="calc-cost-scalper">¥ 1,276 ~ 1,914</div>
                                <div class="text-[10px] text-rose-400">200%-300% 天价溢价</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- SECTION 4: ORDER LOOKUP PORTAL -->
        <section id="orders" class="space-y-6">
            <div class="text-center space-y-2 max-w-xl mx-auto">
                <span class="text-xs font-semibold text-kpink-500 uppercase tracking-wider">Real-time Order Tracking</span>
                <h2 class="text-2xl sm:text-3xl font-bold text-ktext-primary">订单进度查询与状态跟踪</h2>
                <p class="text-xs sm:text-sm text-ktext-secondary">
                    输入订单号（如 IY-2026-8812）或下单时填写的手机/社交账号进行实时检索
                </p>
            </div>

            <div class="max-w-xl mx-auto k-glass p-6 sm:p-8 rounded-4xl border border-kpink-200 shadow-soft space-y-6">
                <div class="flex gap-2">
                    <input type="text" id="search-order-input" placeholder="输入订单号或手机/微信账号" class="flex-grow bg-white border border-kpink-200 rounded-2xl px-4 py-3 text-xs sm:text-sm text-ktext-primary focus:outline-none focus:ring-2 focus:ring-kpink-300">
                    <button onclick="searchOrder()" class="bg-gradient-to-r from-kpink-400 to-kpink-500 text-white font-medium px-6 py-3 rounded-2xl text-xs hover:from-kpink-500 hover:to-kpink-600 transition-all shrink-0">
                        查询状态
                    </button>
                </div>

                <!-- Query Result Box -->
                <div id="order-result-box" class="hidden bg-white p-5 rounded-3xl border border-kpink-100 space-y-4">
                    <div class="flex items-center justify-between border-b border-kpink-100 pb-3">
                        <div>
                            <span class="text-xs font-bold text-ktext-primary" id="res-order-id">#IY-2026-8812</span>
                            <div class="text-[11px] text-ktext-secondary" id="res-show-title">NCT WISH 2nd CONCERT TOUR IN SEOUL</div>
                        </div>
                        <span class="text-xs font-semibold px-3 py-1 rounded-full bg-kpink-100 text-kpink-600" id="res-status-badge">
                            账号已锁定 / 待开售
                        </span>
                    </div>

                    <!-- Progress Steps -->
                    <div class="space-y-3 text-xs">
                        <div class="flex items-start gap-3">
                            <div class="w-5 h-5 rounded-full bg-emerald-500 text-white flex items-center justify-center text-[10px] shrink-0 mt-0.5">✓</div>
                            <div>
                                <div class="font-semibold text-ktext-primary">抢票需求提交与方案锁定</div>
                                <div class="text-[10px] text-ktext-light">客户信息提交成功，第三方退订担保生效</div>
                            </div>
                        </div>
                        <div class="flex items-start gap-3">
                            <div class="w-5 h-5 rounded-full bg-emerald-500 text-white flex items-center justify-center text-[10px] shrink-0 mt-0.5">✓</div>
                            <div>
                                <div class="font-semibold text-ktext-primary">本土实名认证账号完成匹配</div>
                                <div class="text-[10px] text-ktext-light">已分发首尔本土高响应账号</div>
                            </div>
                        </div>
                        <div class="flex items-start gap-3">
                            <div class="w-5 h-5 rounded-full bg-kpink-400 text-white flex items-center justify-center text-[10px] shrink-0 mt-0.5 animate-pulse">3</div>
                            <div>
                                <div class="font-semibold text-kpink-600">等待韩国本土预售窗口开启</div>
                                <div class="text-[10px] text-ktext-secondary">抢票人员已准备完毕，预计开售即刻进入抢订</div>
                            </div>
                        </div>
                        <div class="flex items-start gap-3 opacity-40">
                            <div class="w-5 h-5 rounded-full bg-gray-200 text-gray-500 flex items-center justify-center text-[10px] shrink-0 mt-0.5">4</div>
                            <div>
                                <div class="font-semibold text-ktext-primary">出票凭证确认与尾款结算</div>
                                <div class="text-[10px] text-ktext-light">发送官方订票截图与实体/电子票查验</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- SECTION 5: TRUST & GUARANTEES -->
        <section id="trust" class="space-y-8">
            <div class="text-center space-y-2">
                <span class="text-xs font-semibold text-kpink-500 uppercase tracking-wider">Safety & Service Protocol</span>
                <h2 class="text-2xl sm:text-3xl font-bold text-ktext-primary">服务保障与隐私承诺</h2>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <div class="k-glass p-6 rounded-3xl space-y-3 border border-kpink-200">
                    <div class="w-10 h-10 rounded-2xl bg-kpink-100 flex items-center justify-center text-kpink-600">
                        <i data-lucide="lock" class="w-5 h-5"></i>
                    </div>
                    <h3 class="font-bold text-sm text-ktext-primary">严格个人信息保护</h3>
                    <p class="text-xs text-ktext-secondary leading-relaxed">
                        客户所有身份证照及观演人信息仅用于本次门票实名绑定与官方查验，抢票结束后即刻清空，绝不留存。
                    </p>
                </div>

                <div class="k-glass p-6 rounded-3xl space-y-3 border border-kpink-200">
                    <div class="w-10 h-10 rounded-2xl bg-kpink-100 flex items-center justify-center text-kpink-600">
                        <i data-lucide="user-check" class="w-5 h-5"></i>
                    </div>
                    <h3 class="font-bold text-sm text-ktext-primary">真实本土合规账号</h3>
                    <p class="text-xs text-ktext-secondary leading-relaxed">
                        仅使用在韩留学生持有之本土实名认证账号，避免海外网络封锁，合规抢订，杜绝非法外挂脚本导致的封号风险。
                    </p>
                </div>

                <div class="k-glass p-6 rounded-3xl space-y-3 border border-kpink-200">
                    <div class="w-10 h-10 rounded-2xl bg-kpink-100 flex items-center justify-center text-kpink-600">
                        <i data-lucide="refresh-cw" class="w-5 h-5"></i>
                    </div>
                    <h3 class="font-bold text-sm text-ktext-primary">未出票 100% 全额退款</h3>
                    <p class="text-xs text-ktext-secondary leading-relaxed">
                        若因席位极度紧缺导致未能成功出票，所有定金无条件原路退回，并提供二次转让防诈鉴别指导。
                    </p>
                </div>
            </div>
        </section>

    </main>

    <!-- FOOTER -->
    <footer class="mt-20 bg-white/80 border-t border-kpink-200 py-8 text-center text-xs text-ktext-light z-10 relative">
        <div class="max-w-6xl mx-auto px-4 space-y-3">
            <div class="flex items-center justify-center gap-2 font-bold text-ktext-primary text-sm">
                <span class="w-2 h-2 rounded-full bg-kpink-400"></span>
                IYKYK Ticket Platform
            </div>
            <p class="max-w-xl mx-auto leading-relaxed text-[11px] text-ktext-secondary">
                IYKYK 为海外粉丝提供韩国演唱会本土优先预售协助、抢订及全程协助服务。演出日程及票价来源于 2026 官方公布数据。
            </p>
            <p class="text-[10px] text-ktext-light">
                © 2026 IYKYK Team. All rights reserved.
            </p>
        </div>
    </footer>

    <!-- INTERACTIVE BOOKING MODAL -->
    <div id="booking-modal" class="fixed inset-0 bg-black/40 backdrop-blur-sm z-50 flex items-center justify-center p-4 opacity-0 pointer-events-none transition-opacity duration-300">
        <div class="bg-white w-full max-w-lg rounded-4xl p-6 sm:p-8 shadow-2xl space-y-6 transform scale-95 transition-transform duration-300 max-h-[90vh] overflow-y-auto" id="modal-card">
            
            <div class="flex items-center justify-between border-b border-kpink-100 pb-4">
                <div class="flex items-center gap-2">
                    <div class="w-8 h-8 rounded-full bg-gradient-to-tr from-kpink-400 to-kpink-200 text-white font-bold text-xs flex items-center justify-center">
                        IY
                    </div>
                    <span class="font-bold text-base text-ktext-primary">预订代抢服务</span>
                </div>
                <button onclick="closeBookingModal()" class="text-ktext-light hover:text-ktext-primary p-1">
                    <i data-lucide="x" class="w-5 h-5"></i>
                </button>
            </div>

            <!-- Form -->
            <form id="booking-form" onsubmit="submitBooking(event)" class="space-y-4 text-xs">
                <div class="space-y-1.5">
                    <label class="font-semibold text-ktext-primary">1. 选择演出项目</label>
                    <select id="dw-show" onchange="updateModalPrice()" class="w-full bg-kbg border border-kpink-200 rounded-2xl px-4 py-3 text-ktext-primary focus:outline-none focus:ring-2 focus:ring-kpink-300">
                        <option value="NCT WISH 2nd CONCERT TOUR" data-price="165000">NCT WISH 2nd CONCERT TOUR (高尺巨蛋)</option>
                        <option value="2026 aespa FAN MEETING" data-price="121000">2026 aespa FAN MEETING (高丽大华正)</option>
                        <option value="2026 GISELLE B-day PARTY" data-price="77000">2026 GISELLE B-day PARTY (明和Live Hall)</option>
                        <option value="2026 AND2BLE FAN-CON" data-price="143000">2026 AND2BLE FAN-CON (Tiger Dome)</option>
                        <option value="2026 SUNWOO 粉丝见面会" data-price="99000">2026 SUNWOO 粉丝见面会《UNCHAINED》</option>
                        <option value="2026 CLOSE YOUR EYES FANCON" data-price="121000">2026 CLOSE YOUR EYES FANCON</option>
                        <option value="NMIXX 1ST WORLD TOUR INCHEON" data-price="154000">NMIXX 1ST WORLD TOUR FINALE</option>
                        <option value="2026 CHANYEOL B-day PARTY" data-price="77000">2026 CHANYEOL B-day PARTY</option>
                        <option value="2026 CHENLE B-day PARTY" data-price="77000">2026 CHENLE B-day PARTY [Lele’s Show 2]</option>
                    </select>
                </div>

                <div class="grid grid-cols-2 gap-3">
                    <div class="space-y-1.5">
                        <label class="font-semibold text-ktext-primary">2. 席位偏好</label>
                        <select id="dw-tier" class="w-full bg-kbg border border-kpink-200 rounded-2xl px-3 py-3 text-ktext-primary focus:outline-none focus:ring-2 focus:ring-kpink-300">
                            <option value="VIP 席位 / 内场前排">VIP 席位 / 内场前排</option>
                            <option value="指定席 / 一般看台">指定席 / 一般看台</option>
                            <option value="任意保底席位">任意保底席位</option>
                        </select>
                    </div>
                    <div class="space-y-1.5">
                        <label class="font-semibold text-ktext-primary">3. 张数</label>
                        <select id="dw-qty" class="w-full bg-kbg border border-kpink-200 rounded-2xl px-3 py-3 text-ktext-primary focus:outline-none focus:ring-2 focus:ring-kpink-300">
                            <option value="1">1 张</option>
                            <option value="2">2 张</option>
                        </select>
                    </div>
                </div>

                <div class="space-y-1.5">
                    <label class="font-semibold text-ktext-primary">4. 付费服务方案</label>
                    <select id="dw-plan" onchange="updateModalPrice()" class="w-full bg-kbg border border-kpink-200 rounded-2xl px-4 py-3 text-ktext-primary focus:outline-none focus:ring-2 focus:ring-kpink-300">
                        <option value="Success-First">抢到后付模式 (预付定金 ¥150，出票后结清服务费)</option>
                        <option value="VIP-Priority">VIP 优先锁位方案 (预付定金 ¥300，极速响应)</option>
                    </select>
                </div>

                <div class="space-y-1.5">
                    <label class="font-semibold text-ktext-primary">5. 观演人姓名 (需与护照一致)</label>
                    <input type="text" id="dw-name" required placeholder="如：ZHANG SAN" class="w-full bg-kbg border border-kpink-200 rounded-2xl px-4 py-3 text-ktext-primary placeholder:text-ktext-light focus:outline-none focus:ring-2 focus:ring-kpink-300">
                </div>

                <div class="space-y-1.5">
                    <label class="font-semibold text-ktext-primary">6. 联系方式 (微信 / 手机号 / Telegram)</label>
                    <input type="text" id="dw-contact" required placeholder="抢票成功后第一时间内通知并发送凭证" class="w-full bg-kbg border border-kpink-200 rounded-2xl px-4 py-3 text-ktext-primary placeholder:text-ktext-light focus:outline-none focus:ring-2 focus:ring-kpink-300">
                </div>

                <!-- Price Summary Box -->
                <div class="p-4 rounded-2xl bg-kpink-50/80 border border-kpink-200 space-y-1.5">
                    <div class="flex justify-between items-center text-xs">
                        <span class="text-ktext-secondary">票面估算：</span>
                        <span class="font-medium text-ktext-primary" id="dw-face-val">¥ 638</span>
                    </div>
                    <div class="flex justify-between items-center text-xs">
                        <span class="text-ktext-secondary">本次需付定金：</span>
                        <span class="font-bold text-kpink-600 text-sm" id="dw-deposit-val">¥ 150</span>
                    </div>
                    <div class="text-[10px] text-ktext-light pt-1 border-t border-kpink-200/60">
                        * 未出票定金 100% 全额退还；出票成功后再支付剩余费用。
                    </div>
                </div>

                <button type="submit" class="w-full bg-gradient-to-r from-kpink-400 to-kpink-500 hover:from-kpink-500 hover:to-kpink-600 text-white font-medium py-3.5 rounded-full shadow-soft hover:shadow-soft-lg transition-all text-sm flex items-center justify-center gap-2">
                    <span>确认并提交预订</span>
                    <i data-lucide="arrow-right" class="w-4 h-4"></i>
                </button>
            </form>
        </div>
    </div>

    <!-- TOAST NOTIFICATION -->
    <div id="toast" class="fixed bottom-6 right-6 bg-white/95 border border-kpink-300 px-5 py-3 rounded-2xl shadow-soft text-xs text-ktext-primary flex items-center gap-3 opacity-0 pointer-events-none transition-all duration-300 z-50">
        <span class="w-2 h-2 rounded-full bg-kpink-500 animate-ping"></span>
        <span id="toast-message">提示信息</span>
    </div>

    <!-- JAVASCRIPT LOGIC -->
    <script>
        const concertData = [
            {
                id: 1,
                category: "dome",
                title: "NCT WISH 2nd CONCERT TOUR 'INTO THE WISH' IN SEOUL",
                venue: "GOCHEOK SKY DOME (首尔高尺巨蛋)",
                priceKRW: "VIP席 220,000 / 一般席 165,000 韩元",
                priceRMB: "~ ¥1,160 / ¥870 RMB",
                krPresale: "2026.11.02 (周一) 8:00 PM (KST)",
                globalPresale: "2026.11.03 (周二) 8:00 PM (KST)",
                status: "火热预订中",
                tag: "高尺巨蛋 · 顶级热度"
            },
            {
                id: 2,
                category: "fanmeeting",
                title: "2026 aespa FAN MEETING “MY 보고싶다 ae가”",
                venue: "高丽大学华正体育馆 (Tiger Dome)",
                priceKRW: "指定席 121,000 韩元",
                priceRMB: "~ ¥638 RMB",
                krPresale: "2026.10.27 (周二) 8:00 PM (KST)",
                globalPresale: "2026.10.28 (周三) 8:00 PM (KST)",
                status: "热抢中",
                tag: "粉丝见面会 · 席位紧缺"
            },
            {
                id: 3,
                category: "fanmeeting",
                title: "2026 GISELLE B-day PARTY [In MY Blood]",
                venue: "明和 Live Hall (MYUNGHWA LIVE HALL)",
                priceKRW: "全席统一 77,000 韩元",
                priceRMB: "~ ¥406 RMB",
                krPresale: "2026.10.21 (周三) 8:00 PM (KST)",
                globalPresale: "无 Global 通道 (仅本土独占)",
                status: "本土独占",
                tag: "生日Party · LiveHouse"
            },
            {
                id: 4,
                category: "fanmeeting",
                title: "2026 AND2BLE FAN-CON <W!nter inside> In Seoul",
                venue: "Hwajeong Tiger Dome (华正体育馆)",
                priceKRW: "全席统一 143,000 韩元",
                priceRMB: "~ ¥755 RMB",
                krPresale: "2026.10.21 (周三) 8:00 PM (KST)",
                globalPresale: "2026.10.22 (周四) 8:00 PM (KST)",
                status: "接受预订",
                tag: "FAN-CON · 热门抢购"
            },
            {
                id: 5,
                category: "fanmeeting",
                title: "2026 SUNWOO 粉丝见面会《UNCHAINED》",
                venue: "MYUNGHWA LIVE HALL (明和 Live Hall)",
                priceKRW: "全场统一 99,000 韩元",
                priceRMB: "~ ¥522 RMB",
                krPresale: "2026.10.21 (周三) 8:00 PM (KST)",
                globalPresale: "同步公售通道",
                status: "少量名额",
                tag: "个人FM · 近距离交互"
            },
            {
                id: 6,
                category: "fanmeeting",
                title: "2026 CLOSE YOUR EYES FANCON",
                venue: "Coex Artium WOORI BANK Hall",
                priceKRW: "VIP 121,000 / R席 99,000 韩元",
                priceRMB: "~ ¥638 / ¥522 RMB",
                krPresale: "2026.10.20 (周二) 7:00 PM (KST)",
                globalPresale: "无 Global 通道",
                status: "NOL World 平台",
                tag: "Weverse会员优先"
            },
            {
                id: 7,
                category: "dome",
                title: "NMIXX 1ST WORLD TOUR FINALE IN INCHEON",
                venue: "Inspire Arena (仁川 Inspire 竞技场)",
                priceKRW: "指定座 154,000 韩元",
                priceRMB: "~ ¥812 RMB",
                krPresale: "2026.10.26 (周一) 8:00 PM (KST)",
                globalPresale: "无提前预售",
                status: "世巡终点站",
                tag: "Inspire Arena · 大场馆"
            },
            {
                id: 8,
                category: "fanmeeting",
                title: "2026 CHANYEOL B-day PARTY [B-side]",
                venue: "YES24 LIVE HALL (首尔)",
                priceKRW: "全席统一 77,000 韩元",
                priceRMB: "~ ¥406 RMB",
                krPresale: "2026.10.26 (周一) 8:00 PM (KST)",
                globalPresale: "YES24 Global 通道",
                status: "YES24独占",
                tag: "生日Party · 限量席位"
            },
            {
                id: 9,
                category: "fanmeeting",
                title: "2026 CHENLE B-day PARTY [Lele’s Show 2]",
                venue: "YES24 LIVE HALL (首尔)",
                priceKRW: "全席统一 77,000 韩元",
                priceRMB: "~ ¥406 RMB",
                krPresale: "2026.10.27 (周二) 8:00 PM (KST)",
                globalPresale: "2026.10.28 (周三) 8:00 PM (KST)",
                status: "YES24独占",
                tag: "生日Party · 限量席位"
            }
        ];

        let currentCategory = 'all';

        // Saved active orders
        let userOrders = [
            {
                id: "IY-2026-8812",
                show: "NCT WISH 2nd CONCERT TOUR IN SEOUL",
                contact: "13800138000",
                status: "本土实名账号已锁定 / 待开售"
            }
        ];

        function renderConcerts(data) {
            const container = document.getElementById('concert-grid');
            container.innerHTML = '';

            if(data.length === 0) {
                container.innerHTML = `
                    <div class="col-span-full text-center py-12 text-ktext-light text-xs">
                        未搜寻到匹配的演出，可联系客服添加代抢需求。
                    </div>
                `;
                return;
            }

            data.forEach(item => {
                const card = document.createElement('div');
                card.className = "k-glass rounded-3xl p-6 shadow-card hover:shadow-soft transition-all duration-300 border border-kpink-200/80 flex flex-col justify-between space-y-4 group";
                card.innerHTML = `
                    <div class="space-y-3">
                        <div class="flex items-center justify-between gap-2">
                            <span class="text-[10px] font-semibold px-3 py-1 rounded-full bg-kpink-100 text-kpink-600 border border-kpink-200">
                                ${item.tag}
                            </span>
                            <span class="text-[11px] font-medium text-emerald-600 bg-emerald-50 px-2.5 py-0.5 rounded-full flex items-center gap-1">
                                <span class="w-1.5 h-1.5 rounded-full bg-emerald-500"></span> ${item.status}
                            </span>
                        </div>

                        <h3 class="font-bold text-base text-ktext-primary group-hover:text-kpink-600 transition-colors leading-snug">
                            ${item.title}
                        </h3>

                        <div class="text-xs text-ktext-secondary space-y-1.5 pt-1">
                            <div class="flex items-center gap-2">
                                <i data-lucide="map-pin" class="w-3.5 h-3.5 text-kpink-400 shrink-0"></i>
                                <span>${item.venue}</span>
                            </div>
                            <div class="flex items-center gap-2">
                                <i data-lucide="ticket" class="w-3.5 h-3.5 text-kpink-400 shrink-0"></i>
                                <span class="font-medium text-ktext-primary">${item.priceKRW}</span>
                                <span class="text-ktext-light">(${item.priceRMB})</span>
                            </div>
                        </div>

                        <div class="bg-white/90 rounded-2xl p-3 border border-kpink-100 text-[11px] space-y-1.5 mt-3">
                            <div class="flex items-center justify-between font-medium">
                                <span class="text-kpink-600 flex items-center gap-1">
                                    <i data-lucide="zap" class="w-3 h-3"></i> 韩国本土预售:
                                </span>
                                <span class="text-ktext-primary font-semibold">${item.krPresale}</span>
                            </div>
                            <div class="flex items-center justify-between text-ktext-light">
                                <span>全球 Global 预售:</span>
                                <span>${item.globalPresale}</span>
                            </div>
                        </div>
                    </div>

                    <button onclick="openBookingForShow('${item.title}')" class="w-full mt-2 bg-gradient-to-r from-kpink-400 to-kpink-500 hover:from-kpink-500 hover:to-kpink-600 text-white font-medium py-2.5 rounded-full text-xs shadow-soft transition-all flex items-center justify-center gap-1.5">
                        <span>预订代抢通道</span>
                        <i data-lucide="chevron-right" class="w-3.5 h-3.5"></i>
                    </button>
                `;
                container.appendChild(card);
            });

            lucide.createIcons();
        }

        function filterConcerts() {
            const query = document.getElementById('concert-search').value.toLowerCase().trim();
            
            let filtered = concertData;
            
            if(currentCategory !== 'all') {
                filtered = filtered.filter(item => item.category === currentCategory);
            }

            if(query) {
                filtered = filtered.filter(item => 
                    item.title.toLowerCase().includes(query) || 
                    item.venue.toLowerCase().includes(query)
                );
            }

            renderConcerts(filtered);
        }

        function setCategoryFilter(category) {
            currentCategory = category;
            document.querySelectorAll('.concert-tab').forEach(btn => {
                btn.className = "concert-tab text-ktext-secondary hover:text-ktext-primary px-3.5 py-1 rounded-full transition-all";
            });

            const activeBtn = document.getElementById(`tab-${category}`);
            if(activeBtn) {
                activeBtn.className = "concert-tab bg-kpink-400 text-white px-3.5 py-1 rounded-full transition-all shadow-sm";
            }

            filterConcerts();
        }

        function updateCalculator() {
            const showSelect = document.getElementById('calc-show');
            const krwPrice = parseFloat(showSelect.value);
            const markupRate = parseFloat(document.getElementById('calc-markup').value);

            const rmbTicket = Math.round(krwPrice * 0.00527);
            const serviceFeeRmb = Math.round(rmbTicket * markupRate);
            const totalIykyk = rmbTicket + serviceFeeRmb;

            document.getElementById('calc-cost-face').innerText = `¥ ${rmbTicket}`;
            document.getElementById('calc-cost-iykyk').innerText = `¥ ${totalIykyk}`;
            document.getElementById('calc-fee-detail').innerText = `含服务费 ¥${serviceFeeRmb}`;
            document.getElementById('calc-cost-scalper').innerText = `¥ ${Math.round(rmbTicket*2)} ~ ${Math.round(rmbTicket*3)}`;
        }

        function openBookingModal(planType) {
            if(planType) {
                document.getElementById('dw-plan').value = planType;
            }
            updateModalPrice();
            const modal = document.getElementById('booking-modal');
            const card = document.getElementById('modal-card');
            modal.classList.remove('opacity-0', 'pointer-events-none');
            card.classList.remove('scale-95');
            card.classList.add('scale-100');
        }

        function openBookingForShow(title) {
            const selectEl = document.getElementById('dw-show');
            for(let i=0; i<selectEl.options.length; i++) {
                if(selectEl.options[i].value.includes(title.substring(0, 8))) {
                    selectEl.selectedIndex = i;
                    break;
                }
            }
            openBookingModal();
        }

        function closeBookingModal() {
            const modal = document.getElementById('booking-modal');
            const card = document.getElementById('modal-card');
            card.classList.remove('scale-100');
            card.classList.add('scale-95');
            modal.classList.add('opacity-0', 'pointer-events-none');
        }

        function updateModalPrice() {
            const showSelect = document.getElementById('dw-show');
            const selectedOpt = showSelect.options[showSelect.selectedIndex];
            const krw = parseFloat(selectedOpt.getAttribute('data-price') || "121000");
            const rmb = Math.round(krw * 0.00527);

            const plan = document.getElementById('dw-plan').value;
            const deposit = plan === 'VIP-Priority' ? 300 : 150;

            document.getElementById('dw-face-val').innerText = `¥ ${rmb}`;
            document.getElementById('dw-deposit-val').innerText = `¥ ${deposit}`;
        }

        function submitBooking(e) {
            e.preventDefault();
            const showName = document.getElementById('dw-show').value;
            const contact = document.getElementById('dw-contact').value;
            const name = document.getElementById('dw-name').value;
            
            const newOrderId = `IY-2026-${Math.floor(1000 + Math.random() * 9000)}`;
            
            userOrders.push({
                id: newOrderId,
                show: showName,
                contact: contact,
                name: name,
                status: "实名验证绑定成功 / 等待预售窗口"
            });

            closeBookingModal();
            
            // Search and show updated order result
            document.getElementById('search-order-input').value = newOrderId;
            searchOrder();
            scrollToSection('orders');

            showToast(`预订提交成功！订单号为 ${newOrderId}`);
        }

        function searchOrder() {
            const query = document.getElementById('search-order-input').value.trim();
            const box = document.getElementById('order-result-box');
            
            if(!query) {
                showToast("请输入订单号或预留联系方式");
                return;
            }

            const found = userOrders.find(o => o.id.toLowerCase() === query.toLowerCase() || o.contact.includes(query));

            if(found) {
                document.getElementById('res-order-id').innerText = `#${found.id}`;
                document.getElementById('res-show-title').innerText = found.show;
                document.getElementById('res-status-badge').innerText = found.status;
                box.classList.remove('hidden');
            } else {
                const mockId = query.startsWith('IY') ? query : `IY-2026-${Math.floor(1000 + Math.random()*9000)}`;
                document.getElementById('res-order-id').innerText = mockId;
                document.getElementById('res-show-title').innerText = "韩国本土代抢预订订单";
                document.getElementById('res-status-badge').innerText = "在韩留学生本土账号锁定中";
                box.classList.remove('hidden');
            }
        }

        function scrollToSection(id) {
            const el = document.getElementById(id);
            if(el) {
                el.scrollIntoView({ behavior: 'smooth', block: 'start' });
            }
        }

        function showToast(msg) {
            const toast = document.getElementById('toast');
            document.getElementById('toast-message').innerText = msg;
            toast.classList.remove('opacity-0', 'pointer-events-none');
            setTimeout(() => {
                toast.classList.add('opacity-0', 'pointer-events-none');
            }, 3200);
        }

        window.onload = function() {
            lucide.createIcons();
            renderConcerts(concertData);
            updateCalculator();
        }
    </script>
</body>
</html>
