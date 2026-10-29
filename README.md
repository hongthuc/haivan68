<html lang="vi" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CÔNG TY TNHH ĐẦU TƯ CÔNG NGHỆ VÀ NĂNG LƯỢNG HẢI VÂN 68 - haivan68.vn</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Inter / Montserrat chuẩn Flatsome -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=Montserrat:wght@700;800;900&display=swap" rel="stylesheet">
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        heading: ['Montserrat', 'sans-serif'],
                    },
                    colors: {
                        haivan: {
                            blue: '#164396',
                            darkblue: '#0d2b66',
                            lightblue: '#1e62b8',
                            orange: '#f26522',
                            amber: '#ff9800',
                            yellow: '#ffd600'
                        }
                    }
                }
            }
        }
    </script>

    <style>
        /* Chuẩn khung lưới Flatsome (Row max-width 1200px) để dễ dựng lại trong UX Builder */
        .fs-container {
            max-width: 1200px;
            margin-left: auto;
            margin-right: auto;
            padding-left: 12px;
            padding-right: 12px;
        }
        @media (min-width: 768px) {
            .fs-container {
                padding-left: 15px;
                padding-right: 15px;
            }
        }

        /* Tiêu đề chuẩn Flatsome Title Element (Style Normal / Center) */
        .section-title-container {
            margin-bottom: 1.5rem;
        }
        .section-title-normal {
            display: flex;
            align-items: center;
            justify-content: space-between;
            border-bottom: 2px solid #e5e7eb;
            padding-bottom: 10px;
        }
        .section-title-main {
            position: relative;
            font-weight: 800;
            text-transform: uppercase;
            color: #164396;
        }
        .section-title-main::after {
            content: '';
            position: absolute;
            bottom: -12px;
            left: 0;
            width: 100%;
            height: 3px;
            background: linear-gradient(90deg, #164396, #f26522);
        }

        /* Hiệu ứng mượt cho Box Flatsome */
        .fs-box {
            transition: all 0.25s ease;
        }
        .fs-box:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 25px -5px rgba(22, 67, 150, 0.12);
        }

        /* Nút liên hệ nổi Zalo & Facebook */
        @keyframes pulse-ring {
            0% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(24, 119, 242, 0.6); }
            70% { transform: scale(1); box-shadow: 0 0 0 12px rgba(24, 119, 242, 0); }
            100% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(24, 119, 242, 0); }
        }
        @keyframes pulse-orange {
            0% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(242, 101, 34, 0.7); }
            70% { transform: scale(1); box-shadow: 0 0 0 12px rgba(242, 101, 34, 0); }
            100% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(242, 101, 34, 0); }
        }
        .btn-pulse-blue {
            animation: pulse-ring 2s infinite;
        }
        .btn-pulse-orange {
            animation: pulse-orange 2s infinite;
        }

        /* Ẩn thanh cuộn ngang trên danh mục điện thoại nhưng vẫn vuốt mượt */
        .no-scrollbar::-webkit-scrollbar {
            display: none;
        }
        .no-scrollbar {
            -ms-overflow-style: none;
            scrollbar-width: none;
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 font-sans antialiased selection:bg-haivan-blue selection:text-white">

    <!-- =====================================================================
         HEADER FLATSOME (TOP BAR + HEADER MAIN + HEADER BOTTOM MENU)
         Lưu ý: Dòng trên cùng tuyệt đối không hiển thị tùy chọn UX Builder
    ====================================================================== -->
    <header id="header" class="sticky top-0 z-40 bg-white shadow-sm">
        
        <!-- 1. TOP BAR (Chỉ hiển thị thông tin công ty & liên hệ cho khách hàng) -->
        <div id="top-bar" class="bg-haivan-darkblue text-white text-xs py-2 border-b border-blue-900">
            <div class="fs-container flex flex-wrap items-center justify-between gap-2">
                <div class="flex items-center gap-2 font-medium truncate">
                    <i class="fa-solid fa-solar-panel text-haivan-yellow"></i>
                    <span>CÔNG TY TNHH ĐẦU TƯ CÔNG NGHỆ VÀ NĂNG LƯỢNG HẢI VÂN 68</span>
                    <span class="hidden lg:inline text-blue-300">|</span>
                    <span class="hidden lg:inline text-blue-200"><i class="fa-solid fa-globe mr-1"></i>haivan68.vn</span>
                </div>
                <div class="hidden md:flex items-center gap-4 text-blue-100">
                    <span><i class="fa-solid fa-location-dot text-haivan-amber mr-1"></i>785B Nguyễn Lương Bằng, Phường Hải Vân, TP Đà Nẵng</span>
                    <a href="tel:0911310131" class="font-bold text-haivan-yellow hover:underline">
                        <i class="fa-solid fa-phone-volume mr-1"></i>0911.310.131
                    </a>
                </div>
            </div>
        </div>

        <!-- 2. HEADER MAIN (Logo Hải Vân 68 + Tìm kiếm + Hotline & Mạng xã hội) -->
        <div id="header-main" class="py-3 bg-white border-b border-slate-100">
            <div class="fs-container flex items-center justify-between gap-3 md:gap-6">
                
                <!-- Nút Menu Mobile -->
                <button onclick="toggleMobileMenu()" class="lg:hidden p-2.5 rounded-lg border border-slate-200 text-haivan-blue hover:bg-slate-50" aria-label="Mở danh mục">
                    <i class="fa-solid fa-bars text-xl"></i>
                </button>

                <!-- LOGO HẢI VÂN 68 (Vector SVG tái tạo chuẩn từ file Logo Hải Vân-01.PNG) -->
                <a href="#trang-chu" class="flex items-center gap-2.5 sm:gap-3 group shrink-0">
                    <div class="w-12 h-12 sm:w-14 sm:h-14 flex items-center justify-center">
                        <svg viewBox="0 0 220 220" class="w-full h-full" xmlns="http://www.w3.org/2000/svg">
                            <defs>
                                <linearGradient id="hvBlueGrad" x1="0%" y1="100%" x2="100%" y2="0%">
                                    <stop offset="0%" stop-color="#143280"/>
                                    <stop offset="100%" stop-color="#1a75c4"/>
                                </linearGradient>
                                <linearGradient id="hvOrangeGrad" x1="0%" y1="100%" x2="100%" y2="0%">
                                    <stop offset="0%" stop-color="#e64a19"/>
                                    <stop offset="55%" stop-color="#ff9800"/>
                                    <stop offset="100%" stop-color="#ffeb3b"/>
                                </linearGradient>
                                <linearGradient id="hvSunGrad" x1="0%" y1="0%" x2="100%" y2="100%">
                                    <stop offset="0%" stop-color="#ffd600"/>
                                    <stop offset="100%" stop-color="#e65100"/>
                                </linearGradient>
                            </defs>
                            <!-- Cánh năng lượng xanh dương phía trên - trái -->
                            <path d="M 38 135 L 98 35 C 110 15, 136 15, 148 35 L 162 62 C 148 48, 133 48, 124 62 L 96 108 L 58 108 L 80 135 Z" fill="url(#hvBlueGrad)"/>
                            <path d="M 38 135 L 76 72 L 102 96 L 82 135 Z" fill="url(#hvBlueGrad)"/>
                            <!-- Cánh năng lượng cam vàng phía dưới - phải -->
                            <path d="M 182 85 L 122 185 C 110 205, 84 205, 72 185 L 58 158 C 72 172, 87 172, 96 158 L 124 112 L 162 112 L 140 85 Z" fill="url(#hvOrangeGrad)"/>
                            <path d="M 182 85 L 144 148 L 118 124 L 138 85 Z" fill="url(#hvOrangeGrad)"/>
                            <!-- Tia sáng trắng trung tâm -->
                            <polygon points="110,58 115,92 150,72 122,102 158,110 122,118 150,148 115,128 110,162 105,128 70,148 98,118 62,110 98,102 70,72 105,92" fill="#ffffff"/>
                            <!-- Mặt trời bánh răng ở tâm -->
                            <circle cx="110" cy="110" r="24" fill="#ffffff"/>
                            <circle cx="110" cy="110" r="19" fill="url(#hvSunGrad)" stroke="#ff6d00" stroke-width="2" stroke-dasharray="4 2"/>
                            <circle cx="110" cy="110" r="9" fill="#ffffff"/>
                        </svg>
                    </div>
                    <div class="flex flex-col">
                        <div class="flex items-baseline gap-1.5 font-heading font-black tracking-tight leading-none">
                            <span class="text-xl sm:text-2xl text-haivan-blue">HAI VAN</span>
                            <span class="text-xl sm:text-2xl bg-gradient-to-b from-amber-400 via-orange-500 to-red-600 bg-clip-text text-transparent">68</span>
                        </div>
                        <span class="text-[11px] sm:text-xs text-slate-500 font-medium tracking-wide mt-0.5">Năng lượng xanh bền vững</span>
                    </div>
                </a>

                <!-- Thanh tìm kiếm sản phẩm (Chuẩn Flatsome Search Box) -->
                <div class="hidden md:flex flex-1 max-w-xl">
                    <div class="flex w-full rounded-lg border-2 border-haivan-blue/20 focus-within:border-haivan-blue overflow-hidden bg-slate-50">
                        <select id="desktopSearchCategory" onchange="filterProductsByCategory(this.value)" class="bg-slate-100 text-slate-700 text-xs font-semibold px-3 border-r border-slate-200 focus:outline-none cursor-pointer">
                            <option value="all">Tất cả danh mục</option>
                            <option value="tam-pin">Tấm Pin Mặt Trời</option>
                            <option value="bien-tan">Biến Tần Inverter</option>
                            <option value="pin-luu-tru">Pin Lưu Trữ Lithium</option>
                            <option value="combo-phu-kien">Combo & Phụ Kiện</option>
                        </select>
                        <input id="searchInput" oninput="handleSearchInput(this.value)" type="text" placeholder="Tìm tấm pin Longi, Jinko, biến tần Deye, pin lưu trữ Bettenergy..." class="w-full px-3.5 py-2 text-sm bg-transparent focus:outline-none">
                        <button onclick="scrollToSection('san-pham')" class="bg-haivan-blue hover:bg-haivan-darkblue text-white px-4 text-sm font-semibold transition">
                            <i class="fa-solid fa-magnifying-glass"></i>
                        </button>
                    </div>
                </div>

                <!-- Cụm nút Hotline, Zalo, Facebook trên Header -->
                <div class="flex items-center gap-2 sm:gap-3">
                    <a href="tel:0911310131" class="flex items-center gap-2.5 bg-orange-50 hover:bg-orange-100 border border-orange-200 px-3 py-1.5 rounded-lg transition">
                        <div class="w-8 h-8 rounded-full bg-haivan-orange text-white flex items-center justify-center shrink-0">
                            <i class="fa-solid fa-phone text-sm"></i>
                        </div>
                        <div class="hidden sm:block leading-tight">
                            <span class="block text-[10px] text-slate-500 font-medium uppercase">Hotline tư vấn 24/7</span>
                            <span class="font-bold text-sm text-haivan-orange">0911.310.131</span>
                        </div>
                    </a>

                    <a href="https://zalo.me/0911310131" target="_blank" rel="noopener noreferrer" class="w-9 h-9 rounded-lg bg-blue-600 hover:bg-blue-700 text-white flex items-center justify-center font-bold text-xs shadow-sm transition" title="Chat Zalo 0911.310.131">
                        Zalo
                    </a>

                    <a href="https://www.facebook.com/" target="_blank" rel="noopener noreferrer" class="w-9 h-9 rounded-lg bg-[#1877F2] hover:bg-blue-800 text-white flex items-center justify-center shadow-sm transition" title="Facebook Hải Vân 68">
                        <i class="fa-brands fa-facebook-f text-base"></i>
                    </a>
                </div>
            </div>

            <!-- Thanh tìm kiếm hiển thị trên Điện thoại -->
            <div class="fs-container mt-2.5 md:hidden">
                <div class="flex w-full rounded-lg border border-slate-300 overflow-hidden bg-slate-50">
                    <input oninput="handleSearchInput(this.value)" type="text" placeholder="Tìm sản phẩm điện mặt trời..." class="w-full px-3 py-2 text-xs bg-transparent focus:outline-none">
                    <button onclick="scrollToSection('san-pham')" class="bg-haivan-blue text-white px-3.5 text-xs">
                        <i class="fa-solid fa-magnifying-glass"></i>
                    </button>
                </div>
            </div>
        </div>

        <!-- 3. HEADER BOTTOM - THANH DANH MỤC & MENU NGANG CHUẨN FLATSOME (MÁY TÍNH) -->
        <div id="wide-nav" class="hidden lg:block bg-haivan-blue text-white">
            <div class="fs-container flex items-center justify-between">
                
                <!-- Nút Mega Danh Mục Sản Phẩm (Hover xổ xuống trên máy tính) -->
                <div class="relative group">
                    <button class="flex items-center gap-3 bg-haivan-orange hover:bg-orange-600 text-white font-bold text-xs uppercase tracking-wider px-5 py-3.5 transition">
                        <i class="fa-solid fa-bars-staggered text-sm"></i>
                        <span>DANH MỤC SẢN PHẨM</span>
                        <i class="fa-solid fa-chevron-down text-[10px] ml-2"></i>
                    </button>
                    <!-- Menu danh mục xổ xuống -->
                    <div class="absolute left-0 top-full w-72 bg-white text-slate-800 shadow-xl rounded-b-lg border border-slate-200 opacity-0 invisible group-hover:opacity-100 group-hover:visible transition-all duration-200 z-50 divide-y divide-slate-100">
                        <button onclick="selectCategoryAndScroll('tam-pin')" class="w-full flex items-center justify-between px-4 py-3 text-left text-sm font-medium hover:bg-blue-50 hover:text-haivan-blue transition">
                            <span class="flex items-center gap-2.5"><i class="fa-solid fa-solar-panel text-haivan-blue w-5"></i>Tấm Pin Năng Lượng Mặt Trời</span>
                            <i class="fa-solid fa-angle-right text-xs text-slate-400"></i>
                        </button>
                        <button onclick="selectCategoryAndScroll('bien-tan')" class="w-full flex items-center justify-between px-4 py-3 text-left text-sm font-medium hover:bg-blue-50 hover:text-haivan-blue transition">
                            <span class="flex items-center gap-2.5"><i class="fa-solid fa-microchip text-haivan-orange w-5"></i>Biến Tần Inverter Hòa Lưới & Hybrid</span>
                            <i class="fa-solid fa-angle-right text-xs text-slate-400"></i>
                        </button>
                        <button onclick="selectCategoryAndScroll('pin-luu-tru')" class="w-full flex items-center justify-between px-4 py-3 text-left text-sm font-medium hover:bg-blue-50 hover:text-haivan-blue transition">
                            <span class="flex items-center gap-2.5"><i class="fa-solid fa-car-battery text-emerald-600 w-5"></i>Pin Lưu Trữ Điện Mặt Trời (Lithium)</span>
                            <i class="fa-solid fa-angle-right text-xs text-slate-400"></i>
                        </button>
                        <button onclick="selectCategoryAndScroll('combo-phu-kien')" class="w-full flex items-center justify-between px-4 py-3 text-left text-sm font-medium hover:bg-blue-50 hover:text-haivan-blue transition">
                            <span class="flex items-center gap-2.5"><i class="fa-solid fa-toolbox text-amber-600 w-5"></i>Trọn Gói Lắp Đặt & Tủ Điện Solar</span>
                            <i class="fa-solid fa-angle-right text-xs text-slate-400"></i>
                        </button>
                        <a href="#giai-phap" class="w-full flex items-center justify-between px-4 py-3 text-left text-sm font-medium hover:bg-blue-50 hover:text-haivan-blue transition">
                            <span class="flex items-center gap-2.5"><i class="fa-solid fa-house-signal text-blue-600 w-5"></i>Giải Pháp Điện Mặt Trời Hộ Gia Đình</span>
                            <i class="fa-solid fa-angle-right text-xs text-slate-400"></i>
                        </a>
                        <a href="#giai-phap" class="w-full flex items-center justify-between px-4 py-3 text-left text-sm font-medium hover:bg-blue-50 hover:text-haivan-blue transition">
                            <span class="flex items-center gap-2.5"><i class="fa-solid fa-industry text-indigo-600 w-5"></i>Giải Pháp Điện Mặt Trời Nhà Xưởng</span>
                            <i class="fa-solid fa-angle-right text-xs text-slate-400"></i>
                        </a>
                    </div>
                </div>

                <!-- Menu điều hướng chính -->
                <nav class="flex items-center space-x-1 text-xs font-bold uppercase tracking-wide">
                    <a href="#trang-chu" class="px-4 py-3.5 hover:bg-white/10 transition">Trang chủ</a>
                    <a href="#danh-muc" class="px-4 py-3.5 hover:bg-white/10 transition">Danh mục</a>
                    <a href="#giai-phap" class="px-4 py-3.5 hover:bg-white/10 transition">Giải pháp Điện Mặt Trời</a>
                    <a href="#san-pham" class="px-4 py-3.5 hover:bg-white/10 transition">Sản phẩm</a>
                    <a href="#cong-trinh" class="px-4 py-3.5 hover:bg-white/10 transition">Công trình & Dự án</a>
                    <a href="#tinh-toan" class="px-4 py-3.5 hover:bg-white/10 transition">Báo giá trọn gói</a>
                    <a href="#lien-he" class="px-4 py-3.5 hover:bg-white/10 transition">Liên hệ</a>
                </nav>

                <!-- Cam kết chính hãng -->
                <div class="text-xs text-blue-100 flex items-center gap-2">
                    <i class="fa-solid fa-shield-halved text-haivan-yellow"></i>
                    <span>Bảo hành chính hãng 10 - 25 năm</span>
                </div>
            </div>
        </div>
    </header>

    <!-- =====================================================================
         MENU DRAWER TRÊN ĐIỆN THOẠI (Thiết kế đẹp, trực quan dễ bấm)
    ====================================================================== -->
    <div id="mobileMenuBackdrop" onclick="toggleMobileMenu()" class="fixed inset-0 bg-slate-900/60 z-50 hidden backdrop-blur-xs"></div>
    <aside id="mobileMenuDrawer" class="fixed top-0 left-0 bottom-0 w-80 max-w-[85vw] bg-white z-50 transform -translate-x-full transition-transform duration-300 flex flex-col shadow-2xl">
        <div class="p-4 bg-haivan-blue text-white flex items-center justify-between">
            <div class="font-heading font-extrabold text-base">HẢI VÂN 68 SOLAR</div>
            <button onclick="toggleMobileMenu()" class="w-8 h-8 rounded-lg bg-white/10 flex items-center justify-center text-white">
                <i class="fa-solid fa-xmark"></i>
            </button>
        </div>

        <div class="p-4 overflow-y-auto flex-1 space-y-5">
            <!-- Danh mục sản phẩm trên mobile drawer -->
            <div>
                <div class="text-xs font-bold uppercase text-slate-400 tracking-wider mb-2.5">Danh mục sản phẩm</div>
                <div class="grid grid-cols-1 gap-1.5">
                    <button onclick="selectCategoryMobile('tam-pin')" class="flex items-center gap-3 p-2.5 rounded-lg bg-slate-50 hover:bg-blue-50 text-left text-sm font-semibold text-slate-700">
                        <span class="w-8 h-8 rounded-lg bg-blue-100 text-haivan-blue flex items-center justify-center"><i class="fa-solid fa-solar-panel"></i></span>
                        <span>Tấm Pin Năng Lượng Mặt Trời</span>
                    </button>
                    <button onclick="selectCategoryMobile('bien-tan')" class="flex items-center gap-3 p-2.5 rounded-lg bg-slate-50 hover:bg-blue-50 text-left text-sm font-semibold text-slate-700">
                        <span class="w-8 h-8 rounded-lg bg-orange-100 text-haivan-orange flex items-center justify-center"><i class="fa-solid fa-microchip"></i></span>
                        <span>Biến Tần Inverter</span>
                    </button>
                    <button onclick="selectCategoryMobile('pin-luu-tru')" class="flex items-center gap-3 p-2.5 rounded-lg bg-slate-50 hover:bg-blue-50 text-left text-sm font-semibold text-slate-700">
                        <span class="w-8 h-8 rounded-lg bg-emerald-100 text-emerald-700 flex items-center justify-center"><i class="fa-solid fa-car-battery"></i></span>
                        <span>Pin Lưu Trữ Lithium</span>
                    </button>
                    <button onclick="selectCategoryMobile('combo-phu-kien')" class="flex items-center gap-3 p-2.5 rounded-lg bg-slate-50 hover:bg-blue-50 text-left text-sm font-semibold text-slate-700">
                        <span class="w-8 h-8 rounded-lg bg-amber-100 text-amber-700 flex items-center justify-center"><i class="fa-solid fa-boxes-stacked"></i></span>
                        <span>Combo & Phụ Kiện Solar</span>
                    </button>
                </div>
            </div>

            <!-- Liên kết điều hướng -->
            <div>
                <div class="text-xs font-bold uppercase text-slate-400 tracking-wider mb-2">Menu Trang Web</div>
                <div class="flex flex-col divide-y divide-slate-100 text-sm font-semibold text-slate-700">
                    <a href="#trang-chu" onclick="toggleMobileMenu()" class="py-2.5 hover:text-haivan-blue">Trang chủ</a>
                    <a href="#giai-phap" onclick="toggleMobileMenu()" class="py-2.5 hover:text-haivan-blue">Giải pháp Điện mặt trời (EMP)</a>
                    <a href="#san-pham" onclick="toggleMobileMenu()" class="py-2.5 hover:text-haivan-blue">Sản phẩm Điện mặt trời (DHC)</a>
                    <a href="#cong-trinh" onclick="toggleMobileMenu()" class="py-2.5 hover:text-haivan-blue">Công trình & Dự án Facebook</a>
                    <a href="#tinh-toan" onclick="toggleMobileMenu()" class="py-2.5 hover:text-haivan-blue">Bảng giá lắp đặt trọn gói</a>
                    <a href="#lien-he" onclick="toggleMobileMenu()" class="py-2.5 hover:text-haivan-blue">Liên hệ Hải Vân 68</a>
                </div>
            </div>
        </div>

        <!-- Thông tin chân menu mobile -->
        <div class="p-4 bg-slate-50 border-t border-slate-200 space-y-2 text-xs">
            <div class="font-bold text-haivan-blue">CÔNG TY TNHH ĐẦU TƯ CÔNG NGHỆ VÀ NĂNG LƯỢNG HẢI VÂN 68</div>
            <p class="text-slate-600">Đ/c: 785B Nguyễn Lương Bằng, Phường Hải Vân, TP Đà Nẵng</p>
            <div class="flex gap-2 pt-1">
                <a href="tel:0911310131" class="flex-1 bg-haivan-orange text-white text-center py-2.5 rounded-lg font-bold">
                    <i class="fa-solid fa-phone mr-1"></i>0911.310.131
                </a>
                <a href="https://zalo.me/0911310131" target="_blank" class="flex-1 bg-blue-600 text-white text-center py-2.5 rounded-lg font-bold">
                    Chat Zalo
                </a>
            </div>
        </div>
    </aside>

    <!-- =====================================================================
         MAIN CONTENT (Cấu trúc chuẩn UX Builder: Section -> Row -> Col -> Box)
         Không gắn bất kỳ nhãn dán (sticker/sale badge) nào trên trang chủ
    ====================================================================== -->
    <main id="trang-chu">

        <!-- SECTION 1: BANNER CHÍNH (UX BUILDER: [section] -> [row] -> [col span="7"] + [col span="5"]) -->
        <section class="bg-gradient-to-br from-haivan-darkblue via-haivan-blue to-blue-900 text-white py-8 md:py-14">
            <div class="fs-container">
                <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 md:gap-8 items-center">
                    
                    <!-- Cột trái: Nội dung giới thiệu công ty -->
                    <div class="lg:col-span-7 space-y-4">
                        <p class="text-amber-300 font-semibold text-xs sm:text-sm uppercase tracking-wider">
                            CÔNG TY TNHH ĐẦU TƯ CÔNG NGHỆ VÀ NĂNG LƯỢNG HẢI VÂN 68
                        </p>
                        <h1 class="font-heading font-extrabold text-2xl sm:text-4xl lg:text-[40px] leading-tight">
                            GIẢI PHÁP ĐIỆN MẶT TRỜI HÒA LƯỚI & LƯU TRỮ BỀN VỮNG
                        </h1>
                        <p class="text-blue-100 text-sm sm:text-base leading-relaxed">
                            Chuyên tư vấn, thiết kế, cung cấp vật tư chính hãng và thi công trọn gói hệ thống Điện năng lượng mặt trời cho <strong>Hộ gia đình, Biệt thự, Nhà xưởng và Doanh nghiệp</strong> tại Đà Nẵng & toàn quốc. Giúp tiết kiệm đến 90% chi phí tiền điện hàng tháng và chủ động nguồn điện 24/7.
                        </p>
                        
                        <div class="grid grid-cols-2 sm:grid-cols-3 gap-3 pt-2 text-xs sm:text-sm">
                            <div class="bg-white/10 rounded-lg p-3 border border-white/15">
                                <div class="font-bold text-amber-300 text-base sm:text-lg">Tiết kiệm 90%</div>
                                <div class="text-blue-100">Hóa đơn điện bậc cao</div>
                            </div>
                            <div class="bg-white/10 rounded-lg p-3 border border-white/15">
                                <div class="font-bold text-amber-300 text-base sm:text-lg">Hoàn vốn nhanh</div>
                                <div class="text-blue-100">Chỉ từ 3.5 – 4.5 năm</div>
                            </div>
                            <div class="col-span-2 sm:col-span-1 bg-white/10 rounded-lg p-3 border border-white/15">
                                <div class="font-bold text-amber-300 text-base sm:text-lg">Bảo hành 25 năm</div>
                                <div class="text-blue-100">Hiệu suất tấm pin Tier 1</div>
                            </div>
                        </div>

                        <div class="flex flex-wrap items-center gap-3 pt-3">
                            <a href="tel:0911310131" class="bg-haivan-orange hover:bg-orange-600 text-white font-bold px-5 py-3 rounded-lg text-sm transition flex items-center gap-2 shadow-lg">
                                <i class="fa-solid fa-phone-volume"></i>
                                <span>Tư Vấn Ngay: 0911.310.131</span>
                            </a>
                            <a href="#san-pham" class="bg-white text-haivan-blue hover:bg-blue-50 font-bold px-5 py-3 rounded-lg text-sm transition flex items-center gap-2">
                                <span>Xem Sản Phẩm</span>
                                <i class="fa-solid fa-arrow-right"></i>
                            </a>
                            <a href="#cong-trinh" class="border border-white/40 hover:bg-white/10 text-white font-semibold px-4 py-3 rounded-lg text-sm transition">
                                Xem Dự Án Thi Công
                            </a>
                        </div>
                    </div>

                    <!-- Cột phải: Khung thương hiệu Logo Hải Vân 68 & Ảnh công trình thực tế -->
                    <div class="lg:col-span-5">
                        <div class="bg-white text-slate-800 rounded-xl p-4 sm:p-5 shadow-xl">
                            <div class="flex items-center gap-3 pb-3 mb-3 border-b border-slate-100">
                                <!-- Logo Hải Vân 68 chuẩn -->
                                <div class="w-14 h-14 shrink-0">
                                    <svg viewBox="0 0 220 220" class="w-full h-full" xmlns="http://www.w3.org/2000/svg">
                                        <path d="M 38 135 L 98 35 C 110 15, 136 15, 148 35 L 162 62 C 148 48, 133 48, 124 62 L 96 108 L 58 108 L 80 135 Z" fill="url(#hvBlueGrad)"/>
                                        <path d="M 38 135 L 76 72 L 102 96 L 82 135 Z" fill="url(#hvBlueGrad)"/>
                                        <path d="M 182 85 L 122 185 C 110 205, 84 205, 72 185 L 58 158 C 72 172, 87 172, 96 158 L 124 112 L 162 112 L 140 85 Z" fill="url(#hvOrangeGrad)"/>
                                        <path d="M 182 85 L 144 148 L 118 124 L 138 85 Z" fill="url(#hvOrangeGrad)"/>
                                        <polygon points="110,58 115,92 150,72 122,102 158,110 122,118 150,148 115,128 110,162 105,128 70,148 98,118 62,110 98,102 70,72 105,92" fill="#ffffff"/>
                                        <circle cx="110" cy="110" r="24" fill="#ffffff"/>
                                        <circle cx="110" cy="110" r="19" fill="url(#hvSunGrad)" stroke="#ff6d00" stroke-width="2" stroke-dasharray="4 2"/>
                                        <circle cx="110" cy="110" r="9" fill="#ffffff"/>
                                    </svg>
                                </div>
                                <div>
                                    <div class="font-heading font-black text-lg text-haivan-blue">HAI VAN <span class="text-haivan-orange">68</span></div>
                                    <div class="text-xs text-slate-500">Năng lượng xanh bền vững - haivan68.vn</div>
                                    <div class="text-xs font-semibold text-slate-700 mt-0.5">785B Nguyễn Lương Bằng, P. Hải Vân, Đà Nẵng | ĐT: 0911.310.131</div>
                                </div>
                            </div>
                            <div class="rounded-lg overflow-hidden aspect-[16/10] bg-slate-100">
                                <img src="https://images.unsplash.com/photo-1509391366360-2e959784a276?auto=format&fit=crop&w=900&q=80" 
                                     onerror="this.src='https://placehold.co/800x500/164396/ffffff?text=Dien+Mat+Troi+Hai+Van+68'"
                                     alt="Thi công điện mặt trời Hải Vân 68" 
                                     class="w-full h-full object-cover">
                            </div>
                            <div class="grid grid-cols-3 gap-2 mt-3 text-center text-xs">
                                <div class="bg-slate-50 p-2 rounded border border-slate-100">
                                    <span class="font-bold text-haivan-blue block">LONGi / Jinko</span>
                                    <span class="text-slate-500">Tấm pin Tier 1</span>
                                </div>
                                <div class="bg-slate-50 p-2 rounded border border-slate-100">
                                    <span class="font-bold text-haivan-blue block">Deye / Growatt</span>
                                    <span class="text-slate-500">Biến tần cao cấp</span>
                                </div>
                                <div class="bg-slate-50 p-2 rounded border border-slate-100">
                                    <span class="font-bold text-haivan-blue block">Bettenergy</span>
                                    <span class="text-slate-500">Pin Lithium LFP</span>
                                </div>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </section>

        <!-- =====================================================================
             SECTION 2: DANH MỤC SẢN PHẨM & GIẢI PHÁP (Tối ưu hiển thị đẹp cả trên PC và Điện thoại)
             - Trên Điện thoại: Chia 3 cột x 2 hàng gọn đẹp, icon sắc nét, dễ chạm
             - Trên Máy tính: Chia 6 cột ngang đồng bộ chuẩn Flatsome
        ====================================================================== -->
        <section id="danh-muc" class="py-8 bg-white border-b border-slate-200">
            <div class="fs-container">
                <div class="section-title-container">
                    <div class="section-title-normal">
                        <h2 class="section-title-main text-base sm:text-xl font-heading">
                            DANH MỤC THIẾT BỊ & GIẢI PHÁP
                        </h2>
                        <span class="text-xs text-slate-500 hidden sm:inline">Chọn danh mục để lọc nhanh thiết bị</span>
                    </div>
                </div>

                <!-- Grid Danh mục: 3 cột trên điện thoại, 6 cột trên máy tính -->
                <div class="grid grid-cols-3 md:grid-cols-6 gap-2.5 sm:gap-4">
                    
                    <!-- Danh mục 1 -->
                    <button onclick="selectCategoryAndScroll('tam-pin')" class="fs-box group bg-slate-50 hover:bg-blue-50 border border-slate-200 hover:border-haivan-blue rounded-xl p-3 sm:p-4 text-center flex flex-col items-center justify-center">
                        <div class="w-11 h-11 sm:w-14 sm:h-14 rounded-full bg-blue-100 text-haivan-blue group-hover:bg-haivan-blue group-hover:text-white flex items-center justify-center mb-2 transition">
                            <i class="fa-solid fa-solar-panel text-lg sm:text-2xl"></i>
                        </div>
                        <span class="font-bold text-xs sm:text-sm text-slate-800 group-hover:text-haivan-blue leading-snug">Tấm Pin Mặt Trời</span>
                        <span class="text-[11px] text-slate-500 mt-0.5 hidden sm:block">Jinko, LONGi, Canadian</span>
                    </button>

                    <!-- Danh mục 2 -->
                    <button onclick="selectCategoryAndScroll('bien-tan')" class="fs-box group bg-slate-50 hover:bg-blue-50 border border-slate-200 hover:border-haivan-blue rounded-xl p-3 sm:p-4 text-center flex flex-col items-center justify-center">
                        <div class="w-11 h-11 sm:w-14 sm:h-14 rounded-full bg-orange-100 text-haivan-orange group-hover:bg-haivan-orange group-hover:text-white flex items-center justify-center mb-2 transition">
                            <i class="fa-solid fa-microchip text-lg sm:text-2xl"></i>
                        </div>
                        <span class="font-bold text-xs sm:text-sm text-slate-800 group-hover:text-haivan-blue leading-snug">Biến Tần Inverter</span>
                        <span class="text-[11px] text-slate-500 mt-0.5 hidden sm:block">Deye, Growatt, Solis</span>
                    </button>

                    <!-- Danh mục 3 -->
                    <button onclick="selectCategoryAndScroll('pin-luu-tru')" class="fs-box group bg-slate-50 hover:bg-blue-50 border border-slate-200 hover:border-haivan-blue rounded-xl p-3 sm:p-4 text-center flex flex-col items-center justify-center">
                        <div class="w-11 h-11 sm:w-14 sm:h-14 rounded-full bg-emerald-100 text-emerald-600 group-hover:bg-emerald-600 group-hover:text-white flex items-center justify-center mb-2 transition">
                            <i class="fa-solid fa-car-battery text-lg sm:text-2xl"></i>
                        </div>
                        <span class="font-bold text-xs sm:text-sm text-slate-800 group-hover:text-haivan-blue leading-snug">Pin Lưu Trữ Lithium</span>
                        <span class="text-[11px] text-slate-500 mt-0.5 hidden sm:block">Bettenergy, Pylontech</span>
                    </button>

                    <!-- Danh mục 4 -->
                    <button onclick="selectCategoryAndScroll('combo-phu-kien')" class="fs-box group bg-slate-50 hover:bg-blue-50 border border-slate-200 hover:border-haivan-blue rounded-xl p-3 sm:p-4 text-center flex flex-col items-center justify-center">
                        <div class="w-11 h-11 sm:w-14 sm:h-14 rounded-full bg-amber-100 text-amber-600 group-hover:bg-amber-600 group-hover:text-white flex items-center justify-center mb-2 transition">
                            <i class="fa-solid fa-screwdriver-wrench text-lg sm:text-2xl"></i>
                        </div>
                        <span class="font-bold text-xs sm:text-sm text-slate-800 group-hover:text-haivan-blue leading-snug">Combo & Phụ Kiện</span>
                        <span class="text-[11px] text-slate-500 mt-0.5 hidden sm:block">Tủ điện, Cáp DC, Đèn Solar</span>
                    </button>

                    <!-- Danh mục 5 -->
                    <a href="#giai-phap" class="fs-box group bg-slate-50 hover:bg-blue-50 border border-slate-200 hover:border-haivan-blue rounded-xl p-3 sm:p-4 text-center flex flex-col items-center justify-center">
                        <div class="w-11 h-11 sm:w-14 sm:h-14 rounded-full bg-sky-100 text-sky-600 group-hover:bg-sky-600 group-hover:text-white flex items-center justify-center mb-2 transition">
                            <i class="fa-solid fa-house-chimney-window text-lg sm:text-2xl"></i>
                        </div>
                        <span class="font-bold text-xs sm:text-sm text-slate-800 group-hover:text-haivan-blue leading-snug">Giải Pháp Gia Đình</span>
                        <span class="text-[11px] text-slate-500 mt-0.5 hidden sm:block">Hòa lưới & Lưu trữ 24/7</span>
                    </a>

                    <!-- Danh mục 6 -->
                    <a href="#cong-trinh" class="fs-box group bg-slate-50 hover:bg-blue-50 border border-slate-200 hover:border-haivan-blue rounded-xl p-3 sm:p-4 text-center flex flex-col items-center justify-center">
                        <div class="w-11 h-11 sm:w-14 sm:h-14 rounded-full bg-indigo-100 text-indigo-600 group-hover:bg-indigo-600 group-hover:text-white flex items-center justify-center mb-2 transition">
                            <i class="fa-solid fa-helmet-safety text-lg sm:text-2xl"></i>
                        </div>
                        <span class="font-bold text-xs sm:text-sm text-slate-800 group-hover:text-haivan-blue leading-snug">Dự Án Đã Thi Công</span>
                        <span class="text-[11px] text-slate-500 mt-0.5 hidden sm:block">Hộ dân & Nhà xưởng</span>
                    </a>

                </div>
            </div>
        </section>

        <!-- =====================================================================
             SECTION 3: GIẢI PHÁP ĐIỆN MẶT TRỜI (Theo mẫu https://emp.vn/)
             Cấu trúc Flatsome: [section] -> [row large-columns-4 medium-columns-2 small-columns-1]
        ====================================================================== -->
        <section id="giai-phap" class="py-10 bg-slate-50">
            <div class="fs-container">
                <div class="section-title-container">
                    <div class="section-title-normal">
                        <h2 class="section-title-main text-base sm:text-xl font-heading">
                            GIẢI PHÁP ĐIỆN NĂNG LƯỢNG MẶT TRỜI TOÀN DIỆN
                        </h2>
                        <a href="tel:0911310131" class="text-xs sm:text-sm font-semibold text-haivan-blue hover:text-haivan-orange">
                            Tư vấn kỹ thuật <i class="fa-solid fa-angle-right ml-1"></i>
                        </a>
                    </div>
                </div>

                <!-- 4 Giải pháp trọng tâm theo mẫu EMP.vn -->
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-5">
                    
                    <!-- Giải pháp 1 -->
                    <div class="fs-box bg-white rounded-xl border border-slate-200 overflow-hidden flex flex-col">
                        <div class="aspect-[16/10] bg-slate-100 overflow-hidden">
                            <img src="https://images.unsplash.com/photo-1508514177221-188b1cf16e9d?auto=format&fit=crop&w=700&q=80" 
                                 onerror="this.src='https://placehold.co/600x400/164396/ffffff?text=Dien+Mat+Troi+Gia+Dinh'"
                                 alt="Giải pháp điện mặt trời hòa lưới có lưu trữ cho hộ gia đình" 
                                 class="w-full h-full object-cover">
                        </div>
                        <div class="p-4 flex-1 flex flex-col justify-between">
                            <div>
                                <h3 class="font-bold text-base text-haivan-blue mb-2">
                                    1. Điện Mặt Trời Hòa Lưới Có Lưu Trữ (Hybrid) Hộ Gia Đình
                                </h3>
                                <p class="text-xs sm:text-sm text-slate-600 leading-relaxed mb-3">
                                    Giải pháp kết hợp biến tần Hybrid và bộ pin lưu trữ Lithium giúp duy trì nguồn điện ổn định 24/7 ngay cả khi mất điện lưới. Tăng khả năng tự chủ năng lượng lên đến 85% và xóa nỗi lo giá điện bậc thang leo thang.
                                </p>
                            </div>
                            <ul class="text-xs text-slate-600 space-y-1.5 border-t border-slate-100 pt-3">
                                <li><i class="fa-solid fa-check text-emerald-600 mr-1.5"></i>Chuyển mạch tự động UPS dưới 10ms</li>
                                <li><i class="fa-solid fa-check text-emerald-600 mr-1.5"></i>Hoạt động êm ái, không tiếng ồn</li>
                                <li><i class="fa-solid fa-check text-emerald-600 mr-1.5"></i>Công suất phổ biến: 5kWp – 15kWp</li>
                            </ul>
                        </div>
                    </div>

                    <!-- Giải pháp 2 -->
                    <div class="fs-box bg-white rounded-xl border border-slate-200 overflow-hidden flex flex-col">
                        <div class="aspect-[16/10] bg-slate-100 overflow-hidden">
                            <img src="https://images.unsplash.com/photo-1613665813446-82a78c468a1d?auto=format&fit=crop&w=700&q=80" 
                                 onerror="this.src='https://placehold.co/600x400/164396/ffffff?text=Dien+Mat+Troi+Nha+Xuong'"
                                 alt="Giải pháp điện mặt trời cho doanh nghiệp và nhà xưởng" 
                                 class="w-full h-full object-cover">
                        </div>
                        <div class="p-4 flex-1 flex flex-col justify-between">
                            <div>
                                <h3 class="font-bold text-base text-haivan-blue mb-2">
                                    2. Điện Mặt Trời Áp Mái Cho Doanh Nghiệp & Nhà Xưởng
                                </h3>
                                <p class="text-xs sm:text-sm text-slate-600 leading-relaxed mb-3">
                                    Tận dụng diện tích mái tôn nhà máy, kho xưởng, văn phòng để tạo ra nguồn điện xanh phục vụ sản xuất ban ngày. Cắt giảm mạnh chi phí điện giờ cao điểm và giảm nhiệt độ mái nhà xưởng từ 4 – 6°C.
                                </p>
                            </div>
                            <ul class="text-xs text-slate-600 space-y-1.5 border-t border-slate-100 pt-3">
                                <li><i class="fa-solid fa-check text-emerald-600 mr-1.5"></i>Đạt tiêu chuẩn chứng chỉ xanh quốc tế</li>
                                <li><i class="fa-solid fa-check text-emerald-600 mr-1.5"></i>Mỗi kW tương đương trồng 3 cây xanh</li>
                                <li><i class="fa-solid fa-check text-emerald-600 mr-1.5"></i>Công suất: 30kWp – 1MWp+</li>
                            </ul>
                        </div>
                    </div>

                    <!-- Giải pháp 3 -->
                    <div class="fs-box bg-white rounded-xl border border-slate-200 overflow-hidden flex flex-col">
                        <div class="aspect-[16/10] bg-slate-100 overflow-hidden">
                            <img src="https://images.unsplash.com/photo-1592833159155-c62df1b65634?auto=format&fit=crop&w=700&q=80" 
                                 onerror="this.src='https://placehold.co/600x400/164396/ffffff?text=He+Thong+Luu+Tru+BESS'"
                                 alt="Hệ thống lưu trữ năng lượng ESS và BESS" 
                                 class="w-full h-full object-cover">
                        </div>
                        <div class="p-4 flex-1 flex flex-col justify-between">
                            <div>
                                <h3 class="font-bold text-base text-haivan-blue mb-2">
                                    3. Hệ Thống Lưu Trữ Năng Lượng Công Nghiệp ESS / BESS
                                </h3>
                                <p class="text-xs sm:text-sm text-slate-600 leading-relaxed mb-3">
                                    Giải pháp lưu trữ điện áp cao chuyên dụng cho nhà máy, bệnh viện, khách sạn, resort. Sạc điện vào giờ thấp điểm hoặc từ điện mặt trời dư thừa và xả điện phục vụ tải vào khung giờ cao điểm.
                                </p>
                            </div>
                            <ul class="text-xs text-slate-600 space-y-1.5 border-t border-slate-100 pt-3">
                                <li><i class="fa-solid fa-check text-emerald-600 mr-1.5"></i>Quản lý BMS & PCCC tự động an toàn</li>
                                <li><i class="fa-solid fa-check text-emerald-600 mr-1.5"></i>Ổn định lưới điện, chống sụt áp</li>
                                <li><i class="fa-solid fa-check text-emerald-600 mr-1.5"></i>Dung lượng: 50kWh – 261kWh – 1MWh</li>
                            </ul>
                        </div>
                    </div>

                    <!-- Giải pháp 4 -->
                    <div class="fs-box bg-white rounded-xl border border-slate-200 overflow-hidden flex flex-col">
                        <div class="aspect-[16/10] bg-slate-100 overflow-hidden">
                            <img src="https://images.unsplash.com/photo-1497440001374-f26997328c1b?auto=format&fit=crop&w=700&q=80" 
                                 onerror="this.src='https://placehold.co/600x400/164396/ffffff?text=Giam+Sat+Thong+Minh+24/7'"
                                 alt="Theo dõi và vận hành hệ thống điện mặt trời" 
                                 class="w-full h-full object-cover">
                        </div>
                        <div class="p-4 flex-1 flex flex-col justify-between">
                            <div>
                                <h3 class="font-bold text-base text-haivan-blue mb-2">
                                    4. Giám Sát Hệ Thống Mọi Lúc & Dịch Vụ Vận Hành O&M
                                </h3>
                                <p class="text-xs sm:text-sm text-slate-600 leading-relaxed mb-3">
                                    Theo dõi sản lượng điện mặt trời tạo ra và lượng tiêu thụ theo thời gian thực qua ứng dụng trên điện thoại. Phân tích tối ưu hóa năng lượng, bảo dưỡng vệ sinh định kỳ đảm bảo hiệu suất tối đa.
                                </p>
                            </div>
                            <ul class="text-xs text-slate-600 space-y-1.5 border-t border-slate-100 pt-3">
                                <li><i class="fa-solid fa-check text-emerald-600 mr-1.5"></i>Theo dõi trực tuyến qua App iOS/Android</li>
                                <li><i class="fa-solid fa-check text-emerald-600 mr-1.5"></i>Cảnh báo sự cố tức thì từ xa</li>
                                <li><i class="fa-solid fa-check text-emerald-600 mr-1.5"></i>Dễ dàng mở rộng nâng cấp hệ thống</li>
                            </ul>
                        </div>
                    </div>

                </div>
            </div>
        </section>

        <!-- =====================================================================
             SECTION 4: SẢN PHẨM ĐIỆN MẶT TRỜI (Lấy từ https://www.dhcsolar.com/)
             YÊU CẦU QUAN TRỌNG:
             1. Chia thành 2 cột trên giao diện điện thoại (grid-cols-2)
             2. Chia thành 4 cột trên máy tính (lg:grid-cols-4)
             3. KHÔNG để bất kỳ nhãn dán (sale/hot/new badge) nào trên trang chủ
        ====================================================================== -->
        <section id="san-pham" class="py-10 bg-white">
            <div class="fs-container">
                
                <!-- Tiêu đề + Bộ lọc danh mục sản phẩm -->
                <div class="section-title-container">
                    <div class="flex flex-col md:flex-row md:items-center justify-between gap-3 border-b-2 border-slate-200 pb-3">
                        <h2 class="section-title-main text-base sm:text-xl font-heading">
                            SẢN PHẨM ĐIỆN NĂNG LƯỢNG MẶT TRỜI
                        </h2>
                        <!-- Nút lọc danh mục sản phẩm (Cuộn ngang mượt trên điện thoại) -->
                        <div class="flex items-center gap-1.5 sm:gap-2 overflow-x-auto no-scrollbar py-1">
                            <button onclick="filterProductsByCategory('all')" data-cat-btn="all" class="cat-filter-btn shrink-0 px-3.5 py-1.5 rounded-lg text-xs font-bold bg-haivan-blue text-white transition">
                                Tất cả (16)
                            </button>
                            <button onclick="filterProductsByCategory('tam-pin')" data-cat-btn="tam-pin" class="cat-filter-btn shrink-0 px-3.5 py-1.5 rounded-lg text-xs font-bold bg-slate-100 text-slate-700 hover:bg-slate-200 transition">
                                Tấm Pin Mặt Trời
                            </button>
                            <button onclick="filterProductsByCategory('bien-tan')" data-cat-btn="bien-tan" class="cat-filter-btn shrink-0 px-3.5 py-1.5 rounded-lg text-xs font-bold bg-slate-100 text-slate-700 hover:bg-slate-200 transition">
                                Biến Tần Inverter
                            </button>
                            <button onclick="filterProductsByCategory('pin-luu-tru')" data-cat-btn="pin-luu-tru" class="cat-filter-btn shrink-0 px-3.5 py-1.5 rounded-lg text-xs font-bold bg-slate-100 text-slate-700 hover:bg-slate-200 transition">
                                Pin Lưu Trữ Lithium
                            </button>
                            <button onclick="filterProductsByCategory('combo-phu-kien')" data-cat-btn="combo-phu-kien" class="cat-filter-btn shrink-0 px-3.5 py-1.5 rounded-lg text-xs font-bold bg-slate-100 text-slate-700 hover:bg-slate-200 transition">
                                Combo & Phụ Kiện
                            </button>
                        </div>
                    </div>
                </div>

                <!-- LƯỚI SẢN PHẨM: 2 CỘT TRÊN ĐIỆN THOẠI (grid-cols-2), 4 CỘT TRÊN MÁY TÍNH (lg:grid-cols-4) -->
                <div id="productGrid" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-2.5 sm:gap-5">
                    <!-- Sản phẩm được render tự động từ danh sách thiết bị chuẩn DHC Solar bên dưới -->
                </div>

            </div>
        </section>

        <!-- =====================================================================
             SECTION 5: CÔNG TRÌNH & DỰ ÁN TIÊU BIỂU (Từ Facebook & web mẫu EMP.vn)
             - Giao diện sạch, không nhãn dán đè lên ảnh, dễ thiết kế lại trên UX Builder
        ====================================================================== -->
        <section id="cong-trinh" class="py-10 bg-slate-50 border-t border-slate-200">
            <div class="fs-container">
                <div class="section-title-container">
                    <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-3 border-b-2 border-slate-200 pb-3">
                        <h2 class="section-title-main text-base sm:text-xl font-heading">
                            CÔNG TRÌNH & DỰ ÁN THI CÔNG THỰC TẾ
                        </h2>
                        <div class="flex items-center gap-2 overflow-x-auto no-scrollbar">
                            <button onclick="filterProjects('all')" data-proj-btn="all" class="proj-filter-btn shrink-0 px-3 py-1.5 rounded-lg text-xs font-bold bg-haivan-blue text-white">
                                Tất cả công trình
                            </button>
                            <button onclick="filterProjects('ho-gia-dinh')" data-proj-btn="ho-gia-dinh" class="proj-filter-btn shrink-0 px-3 py-1.5 rounded-lg text-xs font-bold bg-white text-slate-700 border border-slate-200">
                                Hộ gia đình & Biệt thự
                            </button>
                            <button onclick="filterProjects('doanh-nghiep')" data-proj-btn="doanh-nghiep" class="proj-filter-btn shrink-0 px-3 py-1.5 rounded-lg text-xs font-bold bg-white text-slate-700 border border-slate-200">
                                Nhà xưởng & Doanh nghiệp
                            </button>
                        </div>
                    </div>
                </div>

                <!-- Grid Dự án: 1 cột trên màn nhỏ hoặc 2-3 cột chuẩn Flatsome -->
                <div id="projectGrid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-5">
                    <!-- Dự án được render từ dữ liệu bên dưới -->
                </div>
            </div>
        </section>

        <!-- =====================================================================
             SECTION 6: BẢNG GIÁ THAM KHẢO & TÍNH TOÁN HỆ THỐNG ĐIỆN MẶT TRỜI
        ====================================================================== -->
        <section id="tinh-toan" class="py-10 bg-white border-t border-slate-200">
            <div class="fs-container">
                <div class="section-title-container">
                    <div class="section-title-normal">
                        <h2 class="section-title-main text-base sm:text-xl font-heading">
                            BẢNG GIÁ TRỌN GÓI & TƯ VẤN CHỌN CÔNG SUẤT
                        </h2>
                    </div>
                </div>

                <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 items-start">
                    
                    <!-- Cột trái (5 col): Công cụ ước tính công suất theo hóa đơn tiền điện -->
                    <div class="lg:col-span-5 bg-slate-50 rounded-xl p-5 border border-slate-200">
                        <h3 class="font-bold text-base sm:text-lg text-haivan-blue mb-1">
                            Chọn Mức Tiền Điện Hàng Tháng Của Bạn
                        </h3>
                        <p class="text-xs text-slate-500 mb-4">
                            Hệ thống tự động gợi ý cấu hình lắp đặt phù hợp cho gia đình hoặc doanh nghiệp:
                        </p>

                        <div class="space-y-3">
                            <div>
                                <label class="block text-xs font-bold text-slate-700 mb-1.5">Hóa đơn tiền điện trung bình / tháng:</label>
                                <select id="billSelector" onchange="updateSolarCalculator()" class="w-full p-2.5 rounded-lg border border-slate-300 bg-white text-sm font-semibold text-slate-800 focus:outline-none focus:border-haivan-blue">
                                    <option value="2">Từ 1.5 – 2.5 Triệu VNĐ / tháng</option>
                                    <option value="3" selected>Từ 2.5 – 4 Triệu VNĐ / tháng</option>
                                    <option value="5">Từ 4 – 6 Triệu VNĐ / tháng</option>
                                    <option value="10">Từ 8 – 12 Triệu VNĐ / tháng (Biệt thự / Kinh doanh)</option>
                                    <option value="30">Trên 25 Triệu VNĐ / tháng (Nhà xưởng / Doanh nghiệp)</option>
                                </select>
                            </div>

                            <div>
                                <label class="block text-xs font-bold text-slate-700 mb-1.5">Loại hệ thống mong muốn:</label>
                                <select id="systemTypeSelector" onchange="updateSolarCalculator()" class="w-full p-2.5 rounded-lg border border-slate-300 bg-white text-sm font-semibold text-slate-800 focus:outline-none focus:border-haivan-blue">
                                    <option value="hybrid" selected>Hệ Hòa Lưới Có Lưu Trữ (Hybrid - Có điện khi cúp điện)</option>
                                    <option value="ongrid">Hệ Hòa Lưới Bám Tải (Tiết kiệm điện ban ngày)</option>
                                </select>
                            </div>

                            <!-- Kết quả gợi ý -->
                            <div id="calcResultBox" class="bg-white rounded-lg p-4 border border-blue-200 space-y-2.5 mt-3">
                                <div class="flex justify-between text-xs sm:text-sm border-b border-slate-100 pb-2">
                                    <span class="text-slate-500">Công suất khuyến nghị:</span>
                                    <span id="calcKw" class="font-bold text-haivan-blue">Hệ Hybrid 6kWp + Lưu trữ 5kWh</span>
                                </div>
                                <div class="flex justify-between text-xs sm:text-sm border-b border-slate-100 pb-2">
                                    <span class="text-slate-500">Số lượng tấm pin (580W - 650W):</span>
                                    <span id="calcPanels" class="font-semibold text-slate-800">10 tấm pin Tier 1</span>
                                </div>
                                <div class="flex justify-between text-xs sm:text-sm border-b border-slate-100 pb-2">
                                    <span class="text-slate-500">Sản lượng điện tạo ra / tháng:</span>
                                    <span id="calcOutput" class="font-semibold text-emerald-600">720 – 850 kWh/tháng</span>
                                </div>
                                <div class="flex justify-between text-xs sm:text-sm border-b border-slate-100 pb-2">
                                    <span class="text-slate-500">Diện tích mái cần thiết:</span>
                                    <span id="calcArea" class="font-semibold text-slate-800">~ 26 m²</span>
                                </div>
                                <div class="flex justify-between items-center pt-1">
                                    <span class="text-xs font-bold text-slate-700">Chi phí đầu tư tham khảo:</span>
                                    <span id="calcPrice" class="font-extrabold text-base text-haivan-orange">75.000.000 – 85.000.000 ₫</span>
                                </div>
                            </div>

                            <div class="pt-2 flex gap-2">
                                <a href="tel:0911310131" class="flex-1 bg-haivan-orange hover:bg-orange-600 text-white text-center font-bold py-2.5 rounded-lg text-xs sm:text-sm transition">
                                    <i class="fa-solid fa-phone mr-1"></i>Gọi Nhận Báo Giá Chi Tiết
                                </a>
                                <a href="https://zalo.me/0911310131" target="_blank" class="bg-blue-600 hover:bg-blue-700 text-white font-bold px-4 py-2.5 rounded-lg text-xs sm:text-sm transition">
                                    Zalo
                                </a>
                            </div>
                        </div>
                    </div>

                    <!-- Cột phải (7 col): Bảng giá các gói lắp đặt tiêu chuẩn -->
                    <div class="lg:col-span-7 overflow-x-auto">
                        <div class="bg-white rounded-xl border border-slate-200 overflow-hidden">
                            <table class="w-full text-left border-collapse text-xs sm:text-sm">
                                <thead>
                                    <tr class="bg-haivan-blue text-white">
                                        <th class="p-3 font-bold">Gói Hệ Thống Điện Mặt Trời</th>
                                        <th class="p-3 font-bold">Số tấm pin</th>
                                        <th class="p-3 font-bold">Sản lượng/tháng</th>
                                        <th class="p-3 font-bold">Giá tham khảo (VNĐ)</th>
                                    </tr>
                                </thead>
                                <tbody class="divide-y divide-slate-200">
                                    <tr class="hover:bg-slate-50">
                                        <td class="p-3 font-semibold text-slate-800">Hệ Hòa Lưới 5kWp 1 Pha Gia Đình</td>
                                        <td class="p-3 text-slate-600">8 - 9 tấm</td>
                                        <td class="p-3 text-slate-600">600 - 700 kWh</td>
                                        <td class="p-3 font-bold text-haivan-orange">48 – 55 triệu</td>
                                    </tr>
                                    <tr class="hover:bg-slate-50">
                                        <td class="p-3 font-semibold text-slate-800">Hệ Hybrid 5kWp + Pin Lithium 5kWh</td>
                                        <td class="p-3 text-slate-600">9 tấm</td>
                                        <td class="p-3 text-slate-600">650 - 750 kWh</td>
                                        <td class="p-3 font-bold text-haivan-orange">72 – 82 triệu</td>
                                    </tr>
                                    <tr class="hover:bg-slate-50">
                                        <td class="p-3 font-semibold text-slate-800">Hệ Hybrid 6kWp + Pin Lithium 10kWh</td>
                                        <td class="p-3 text-slate-600">10 - 11 tấm</td>
                                        <td class="p-3 text-slate-600">750 - 900 kWh</td>
                                        <td class="p-3 font-bold text-haivan-orange">95 – 110 triệu</td>
                                    </tr>
                                    <tr class="hover:bg-slate-50">
                                        <td class="p-3 font-semibold text-slate-800">Hệ Hybrid 10kWp 3 Pha + Lưu trữ 15kWh</td>
                                        <td class="p-3 text-slate-600">16 - 18 tấm</td>
                                        <td class="p-3 text-slate-600">1.200 - 1.450 kWh</td>
                                        <td class="p-3 font-bold text-haivan-orange">145 – 168 triệu</td>
                                    </tr>
                                    <tr class="hover:bg-slate-50">
                                        <td class="p-3 font-semibold text-slate-800">Hệ Có Lưu Trữ 30kW 3 Pha (Doanh nghiệp)</td>
                                        <td class="p-3 text-slate-600">50 tấm</td>
                                        <td class="p-3 text-slate-600">3.600 - 4.200 kWh</td>
                                        <td class="p-3 font-bold text-haivan-orange">390 – 420 triệu</td>
                                    </tr>
                                    <tr class="hover:bg-slate-50">
                                        <td class="p-3 font-semibold text-slate-800">Hệ Có Lưu Trữ 50kW – 100kW Nhà Xưởng</td>
                                        <td class="p-3 text-slate-600">85 - 165 tấm</td>
                                        <td class="p-3 text-slate-600">6.500 - 13.500 kWh</td>
                                        <td class="p-3 font-bold text-haivan-orange">650 triệu – 1.4 tỷ</td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>
                        <p class="text-xs text-slate-500 mt-2.5">
                            * Báo giá đã bao gồm tấm pin năng lượng mặt trời chính hãng (LONGi, Jinko, Canadian, AE Solar), biến tần Inverter, pin lưu trữ Lithium, khung giàn nhôm định hình chống rỉ, tủ điện bảo vệ AC/DC và nhân công lắp đặt trọn gói của <strong>Hải Vân 68</strong>.
                        </p>
                    </div>

                </div>
            </div>
        </section>

    </main>

    <!-- =====================================================================
         FOOTER FLATSOME (Đầy đủ thông tin pháp lý Hải Vân 68, Địa chỉ, SĐT, Website)
    ====================================================================== -->
    <footer id="lien-he" class="bg-haivan-darkblue text-white pt-12 pb-6 border-t-4 border-haivan-orange">
        <div class="fs-container">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-12 gap-8 pb-8 border-b border-blue-800/80">
                
                <!-- Cột 1 (5 col): Thông tin công ty & Logo -->
                <div class="lg:col-span-5 space-y-3">
                    <div class="flex items-center gap-3 bg-white p-3 rounded-xl w-fit">
                        <div class="w-11 h-11">
                            <svg viewBox="0 0 220 220" class="w-full h-full" xmlns="http://www.w3.org/2000/svg">
                                <path d="M 38 135 L 98 35 C 110 15, 136 15, 148 35 L 162 62 C 148 48, 133 48, 124 62 L 96 108 L 58 108 L 80 135 Z" fill="url(#hvBlueGrad)"/>
                                <path d="M 38 135 L 76 72 L 102 96 L 82 135 Z" fill="url(#hvBlueGrad)"/>
                                <path d="M 182 85 L 122 185 C 110 205, 84 205, 72 185 L 58 158 C 72 172, 87 172, 96 158 L 124 112 L 162 112 L 140 85 Z" fill="url(#hvOrangeGrad)"/>
                                <path d="M 182 85 L 144 148 L 118 124 L 138 85 Z" fill="url(#hvOrangeGrad)"/>
                                <polygon points="110,58 115,92 150,72 122,102 158,110 122,118 150,148 115,128 110,162 105,128 70,148 98,118 62,110 98,102 70,72 105,92" fill="#ffffff"/>
                                <circle cx="110" cy="110" r="24" fill="#ffffff"/>
                                <circle cx="110" cy="110" r="19" fill="url(#hvSunGrad)" stroke="#ff6d00" stroke-width="2" stroke-dasharray="4 2"/>
                                <circle cx="110" cy="110" r="9" fill="#ffffff"/>
                            </svg>
                        </div>
                        <div>
                            <div class="font-heading font-black text-lg text-haivan-blue leading-none">HAI VAN <span class="text-haivan-orange">68</span></div>
                            <div class="text-[11px] text-slate-500 font-medium mt-0.5">Năng lượng xanh bền vững</div>
                        </div>
                    </div>

                    <h3 class="font-bold text-sm sm:text-base text-amber-300 pt-1">
                        CÔNG TY TNHH ĐẦU TƯ CÔNG NGHỆ VÀ NĂNG LƯỢNG HẢI VÂN 68
                    </h3>
                    <ul class="space-y-2 text-xs sm:text-sm text-blue-100">
                        <li class="flex items-start gap-2.5">
                            <i class="fa-solid fa-location-dot text-haivan-amber mt-1 shrink-0"></i>
                            <span><strong>Địa chỉ:</strong> 785B Nguyễn Lương Bằng, Phường Hải Vân, TP Đà Nẵng</span>
                        </li>
                        <li class="flex items-center gap-2.5">
                            <i class="fa-solid fa-phone-volume text-haivan-amber shrink-0"></i>
                            <span><strong>Điện thoại / Zalo:</strong> <a href="tel:0911310131" class="text-white font-bold hover:underline">0911.310.131</a></span>
                        </li>
                        <li class="flex items-center gap-2.5">
                            <i class="fa-solid fa-globe text-haivan-amber shrink-0"></i>
                            <span><strong>Website:</strong> <a href="https://haivan68.vn" class="text-white hover:underline">haivan68.vn</a></span>
                        </li>
                    </ul>
                </div>

                <!-- Cột 2 (3 col): Giải pháp & Sản phẩm -->
                <div class="lg:col-span-3 space-y-2.5">
                    <h4 class="font-bold text-sm uppercase tracking-wider text-amber-300">Danh Mục & Giải Pháp</h4>
                    <ul class="space-y-2 text-xs sm:text-sm text-blue-100">
                        <li><a href="#san-pham" onclick="filterProductsByCategory('tam-pin')" class="hover:text-white">› Tấm Pin Năng Lượng Mặt Trời</a></li>
                        <li><a href="#san-pham" onclick="filterProductsByCategory('bien-tan')" class="hover:text-white">› Biến Tần Hòa Lưới & Hybrid</a></li>
                        <li><a href="#san-pham" onclick="filterProductsByCategory('pin-luu-tru')" class="hover:text-white">› Pin Lưu Trữ Lithium Bettenergy</a></li>
                        <li><a href="#giai-phap" class="hover:text-white">› Giải Pháp Điện Mặt Trời Hộ Gia Đình</a></li>
                        <li><a href="#giai-phap" class="hover:text-white">› Giải Pháp Điện Mặt Trời Nhà Xưởng</a></li>
                        <li><a href="#cong-trinh" class="hover:text-white">› Dự Án Điện Mặt Trời Tiêu Biểu</a></li>
                    </ul>
                </div>

                <!-- Cột 3 (4 col): Kết nối Zalo, Facebook & Nhận báo giá -->
                <div class="lg:col-span-4 space-y-3">
                    <h4 class="font-bold text-sm uppercase tracking-wider text-amber-300">Liên Hệ Tư Vấn Trực Tiếp</h4>
                    <p class="text-xs sm:text-sm text-blue-100 leading-relaxed">
                        Quý khách cần khảo sát mái nhà, tư vấn lắp đặt điện mặt trời tại Đà Nẵng và khu vực miền Trung vui lòng liên hệ trực tiếp qua Zalo hoặc Facebook của Hải Vân 68:
                    </p>
                    <div class="flex flex-wrap gap-2.5 pt-1">
                        <a href="https://zalo.me/0911310131" target="_blank" rel="noopener noreferrer" class="flex items-center gap-2 bg-blue-600 hover:bg-blue-500 text-white font-bold text-xs px-4 py-2.5 rounded-lg transition">
                            <i class="fa-solid fa-comment-dots"></i>
                            <span>Chat Zalo: 0911.310.131</span>
                        </a>
                        <a href="https://www.facebook.com/" target="_blank" rel="noopener noreferrer" class="flex items-center gap-2 bg-[#1877F2] hover:bg-blue-700 text-white font-bold text-xs px-4 py-2.5 rounded-lg transition">
                            <i class="fa-brands fa-facebook"></i>
                            <span>Facebook Hải Vân 68</span>
                        </a>
                    </div>
                    <div class="pt-2">
                        <button onclick="openUxShortcodeModal()" class="text-xs text-blue-200 hover:text-white underline flex items-center gap-1.5">
                            <i class="fa-solid fa-code"></i>
                            <span>Xem mã Shortcode chuẩn UX Builder Flatsome</span>
                        </button>
                    </div>
                </div>

            </div>

            <div class="fs-container pt-5 flex flex-col sm:flex-row items-center justify-between text-xs text-blue-200 gap-2">
                <div>© Bản quyền thuộc về <strong>CÔNG TY TNHH ĐẦU TƯ CÔNG NGHỆ VÀ NĂNG LƯỢNG HẢI VÂN 68</strong> (haivan68.vn)</div>
                <div>Thiết kế chuẩn bố cục Flatsome – Tối ưu Điện thoại & Máy tính</div>
            </div>
        </footer>
    </footer>

    <!-- =====================================================================
         CỤM NÚT LIÊN HỆ NỔI (ZALO, FACEBOOK, GỌI ĐIỆN) CỐ ĐỊNH GÓC MÀN HÌNH
    ====================================================================== -->
    <div class="fixed bottom-4 right-4 z-40 flex flex-col items-end gap-2.5">
        
        <!-- Nút Facebook -->
        <a href="https://www.facebook.com/" target="_blank" rel="noopener noreferrer" 
           class="flex items-center gap-2 bg-[#1877F2] hover:bg-blue-700 text-white px-3.5 py-2.5 rounded-full shadow-lg transition group"
           title="Liên hệ qua Facebook">
            <i class="fa-brands fa-facebook-f text-base w-5 text-center"></i>
            <span class="text-xs font-bold pr-1">Facebook</span>
        </a>

        <!-- Nút Zalo -->
        <a href="https://zalo.me/0911310131" target="_blank" rel="noopener noreferrer" 
           class="btn-pulse-blue flex items-center gap-2 bg-blue-600 hover:bg-blue-700 text-white px-3.5 py-2.5 rounded-full shadow-lg transition"
           title="Chat Zalo 0911.310.131">
            <span class="w-5 h-5 rounded-full bg-white text-blue-600 font-black text-[10px] flex items-center justify-center">Z</span>
            <span class="text-xs font-bold pr-1">Chat Zalo</span>
        </a>

        <!-- Nút Gọi Hotline -->
        <a href="tel:0911310131" 
           class="btn-pulse-orange flex items-center gap-2 bg-haivan-orange hover:bg-orange-600 text-white px-4 py-2.5 rounded-full shadow-lg transition"
           title="Gọi 0911.310.131">
            <i class="fa-solid fa-phone-volume text-sm"></i>
            <span class="text-xs sm:text-sm font-extrabold">0911.310.131</span>
        </a>

    </div>

    <!-- =====================================================================
         MODAL CHI TIẾT SẢN PHẨM / BÁO GIÁ NHANH (KHÔNG DÙNG ALERT)
    ====================================================================== -->
    <div id="productModal" class="fixed inset-0 bg-slate-900/60 z-50 hidden items-center justify-center p-4 backdrop-blur-xs">
        <div class="bg-white rounded-xl max-w-lg w-full overflow-hidden shadow-2xl border border-slate-200">
            <div class="p-4 bg-haivan-blue text-white flex items-center justify-between">
                <h3 id="modalTitle" class="font-bold text-sm sm:text-base truncate pr-4">Thông tin sản phẩm</h3>
                <button onclick="closeProductModal()" class="w-8 h-8 rounded-lg bg-white/10 hover:bg-white/20 flex items-center justify-center">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>
            <div class="p-4 sm:p-5 space-y-4">
                <div class="flex gap-4 items-center">
                    <img id="modalImage" src="" alt="" class="w-24 h-24 rounded-lg object-cover border border-slate-200 shrink-0">
                    <div>
                        <div id="modalCategory" class="text-xs text-slate-500 font-medium">Danh mục</div>
                        <div id="modalPrice" class="text-lg font-extrabold text-haivan-orange mt-1">Liên hệ</div>
                        <div id="modalSpec" class="text-xs text-slate-600 mt-1">Chính hãng CO/CQ đầy đủ</div>
                    </div>
                </div>
                <p id="modalDesc" class="text-xs sm:text-sm text-slate-600 leading-relaxed bg-slate-50 p-3 rounded-lg border border-slate-100"></p>
                <div class="text-xs text-slate-500 space-y-1">
                    <div><strong class="text-slate-700">Đơn vị phân phối & thi công:</strong> CÔNG TY TNHH ĐẦU TƯ CÔNG NGHỆ VÀ NĂNG LƯỢNG HẢI VÂN 68</div>
                    <div><strong class="text-slate-700">Địa chỉ:</strong> 785B Nguyễn Lương Bằng, Phường Hải Vân, TP Đà Nẵng</div>
                </div>
                <div class="grid grid-cols-2 gap-2.5 pt-2">
                    <a href="tel:0911310131" class="bg-haivan-orange hover:bg-orange-600 text-white text-center font-bold py-2.5 rounded-lg text-xs sm:text-sm transition">
                        <i class="fa-solid fa-phone mr-1"></i>Gọi 0911.310.131
                    </a>
                    <a href="https://zalo.me/0911310131" target="_blank" class="bg-blue-600 hover:bg-blue-700 text-white text-center font-bold py-2.5 rounded-lg text-xs sm:text-sm transition">
                        <i class="fa-solid fa-comment-dots mr-1"></i>Nhắn Zalo Báo Giá
                    </a>
                </div>
            </div>
        </div>
    </div>

    <!-- =====================================================================
         MODAL SHORTCODE FLATSOME UX BUILDER (Hỗ trợ copy dán nhanh vào WordPress)
    ====================================================================== -->
    <div id="uxShortcodeModal" class="fixed inset-0 bg-slate-900/60 z-50 hidden items-center justify-center p-4 backdrop-blur-xs">
        <div class="bg-white rounded-xl max-w-2xl w-full overflow-hidden shadow-2xl border border-slate-200">
            <div class="p-4 bg-haivan-darkblue text-white flex items-center justify-between">
                <h3 class="font-bold text-sm sm:text-base"><i class="fa-solid fa-Layer-group mr-2"></i>Mã Shortcode Chuẩn UX Builder Flatsome (Copy dán vào Trang Chủ)</h3>
                <button onclick="closeUxShortcodeModal()" class="w-8 h-8 rounded-lg bg-white/10 hover:bg-white/20 flex items-center justify-center">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>
            <div class="p-4 space-y-3">
                <p class="text-xs text-slate-600">
                    Toàn bộ giao diện trang chủ đã được chia theo đúng cấu trúc <strong>Section &rarr; Row &rarr; Col &rarr; UX Products (2 cột trên điện thoại, 4 cột trên máy tính)</strong> của Flatsome. Bạn có thể copy đoạn Shortcode dưới đây dán thẳng vào trình sửa văn bản của UX Builder:
                </p>
                <textarea id="uxShortcodeText" readonly class="w-full h-56 p-3 text-xs font-mono bg-slate-900 text-emerald-400 rounded-lg focus:outline-none">[section label="Banner Hai Van 68" bg_color="#164396" dark="true" padding="50px"]
[row style="large" v_align="middle"]
[col span="7" span__sm="12"]
[ux_html]
<h4>CÔNG TY TNHH ĐẦU TƯ CÔNG NGHỆ VÀ NĂNG LƯỢNG HẢI VÂN 68</h4>
<h1>GIẢI PHÁP ĐIỆN MẶT TRỜI HÒA LƯỚI & LƯU TRỮ BỀN VỮNG</h1>
<p>Địa chỉ: 785B Nguyễn Lương Bằng, Phường Hải Vân, TP Đà Nẵng | Hotline: 0911.310.131</p>
[/ux_html]
[button text="Tư vấn: 0911.310.131" color="alert" link="tel:0911310131"]
[button text="Xem sản phẩm" color="white" style="outline" link="#san-pham"]
[/col]
[col span="5" span__sm="12"]
[ux_image id="" image_size="original"]
[/col]
[/row]
[/section]

[section label="Danh Muc San Pham" padding="40px"]
[row]
[col span="12"]
[title style="normal" text="DANH MỤC THIẾT BỊ & GIẢI PHÁP" tag_name="h2"]
[ux_product_categories style="normal" type="row" columns="6" columns__sm="3" show_count="0"]
[/col]
[/row]
[/section]

[section label="Giai Phap EMP" bg_color="#f8fafc" padding="40px"]
[row]
[col span="12"]
[title style="normal" text="GIẢI PHÁP ĐIỆN NĂNG LƯỢNG MẶT TRỜI" tag_name="h2"]
[/col]
[/row]
[row columns="4" columns__md="2" columns__sm="1"]
[col span="3" span__sm="12"][featured_box title="1. Hòa lưới có lưu trữ Gia đình"]Chủ động nguồn điện 24/7 khi cúp điện, tiết kiệm 85-90% tiền điện.[/featured_box][/col]
[col span="3" span__sm="12"][featured_box title="2. Điện mặt trời Nhà xưởng"]Giảm chi phí điện giờ cao điểm, làm mát mái nhà máy 4-6 độ C.[/featured_box][/col]
[col span="3" span__sm="12"][featured_box title="3. Hệ thống lưu trữ BESS"]Lưu trữ năng lượng công nghiệp áp cao 50kWh - 1MWh an toàn.[/featured_box][/col]
[col span="3" span__sm="12"][featured_box title="4. Giám sát thông minh 24/7"]Theo dõi sản lượng điện trực tuyến qua điện thoại mọi lúc.[/featured_box][/col]
[/row]
[/section]

[section label="San Pham DHC Solar" padding="40px"]
[row]
[col span="12"]
[title style="normal" text="SẢN PHẨM ĐIỆN NĂNG LƯỢNG MẶT TRỜI" tag_name="h2"]
[ux_products style="normal" type="row" columns="4" columns__sm="2" products="16" show_cat="0" show_quick_view="0"]
[/col]
[/row]
[/section]

[section label="Cong Trinh Du An" bg_color="#f8fafc" padding="40px"]
[row]
[col span="12"]
[title style="normal" text="CÔNG TRÌNH & DỰ ÁN THI CÔNG THỰC TẾ" tag_name="h2"]
[blog_posts style="normal" type="row" columns="3" columns__sm="1" posts="6" show_date="false" badge_style="none"]
[/col]
[/row]
[/section]</textarea>
                <div class="flex items-center justify-between">
                    <span id="copyConfirmMsg" class="text-xs font-semibold text-emerald-600 hidden"><i class="fa-solid fa-check mr-1"></i>Đã sao chép Shortcode vào bộ nhớ tạm!</span>
                    <div class="flex gap-2 ml-auto">
                        <button onclick="copyUxShortcode()" class="bg-haivan-blue hover:bg-haivan-darkblue text-white text-xs font-bold px-4 py-2 rounded-lg">
                            <i class="fa-solid fa-copy mr-1"></i>Sao chép Shortcode
                        </button>
                        <button onclick="closeUxShortcodeModal()" class="bg-slate-200 hover:bg-slate-300 text-slate-700 text-xs font-bold px-4 py-2 rounded-lg">
                            Đóng
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- =====================================================================
         JAVASCRIPT XỬ LÝ DỮ LIỆU SẢN PHẨM (DHC SOLAR) & DỰ ÁN (EMP / FACEBOOK)
    ====================================================================== -->
    <script>
        // 1. Danh sách 16 sản phẩm lấy từ danh mục thực tế của dhcsolar.com
        // Tuyệt đối không gắn nhãn dán (sticker/sale badge) trên thẻ sản phẩm trang chủ
        const productsData = [
            // TẤM PIN NĂNG LƯỢNG MẶT TRỜI
            {
                id: 1,
                name: "Tấm Pin Jinko Solar Tiger Neo 585W N-Type",
                category: "tam-pin",
                categoryLabel: "Tấm Pin Mặt Trời",
                price: "2.400.000 ₫",
                spec: "Công suất: 585Wp | N-Type TOPCon | BH 12 năm",
                image: "https://images.unsplash.com/photo-1509391366360-2e959784a276?auto=format&fit=crop&w=600&q=80",
                desc: "Tấm pin năng lượng mặt trời Jinko Solar 585W công nghệ N-Type TOPCon thế hệ mới, hiệu suất chuyển đổi cao trên 22.6%, hoạt động vượt trội trong điều kiện bức xạ yếu."
            },
            {
                id: 2,
                name: "Tấm Pin LONGi Hi-MO X10 650W Công Suất Cao",
                category: "tam-pin",
                categoryLabel: "Tấm Pin Mặt Trời",
                price: "2.730.000 ₫",
                spec: "Công suất: 650Wp | Công nghệ HPBC 2.0",
                image: "https://images.unsplash.com/photo-1508514177221-188b1cf16e9d?auto=format&fit=crop&w=600&q=80",
                desc: "Tấm pin năng lượng mặt trời LONGi Hi-MO X10 650W chính hãng, không đường hàn mặt trước giúp tối ưu khả năng hấp thụ ánh sáng và chống rạn nứt vi mô."
            },
            {
                id: 3,
                name: "Tấm Pin Canadian Solar 550W HiKu6 Mono PERC",
                category: "tam-pin",
                categoryLabel: "Tấm Pin Mặt Trời",
                price: "1.760.000 ₫",
                spec: "Công suất: 550Wp | Mono Half-Cell",
                image: "https://images.unsplash.com/photo-1613665813446-82a78c468a1d?auto=format&fit=crop&w=600&q=80",
                desc: "Tấm pin mặt trời Canadian 550W thương hiệu Canada thuộc Top Tier 1 thế giới, khung nhôm аноdized chịu tải gió bão lớn tại khu vực miền Trung."
            },
            {
                id: 4,
                name: "Tấm Pin AE Solar 580W N-Type TOPCon Đức",
                category: "tam-pin",
                categoryLabel: "Tấm Pin Mặt Trời",
                price: "1.740.000 ₫",
                spec: "Công suất: 580Wp | Thương hiệu Đức",
                image: "https://images.unsplash.com/photo-1559302504-64aae6ca6b6d?auto=format&fit=crop&w=600&q=80",
                desc: "Tấm pin AE Solar 580W công nghệ N-Type chống suy giảm hiệu suất LID/PID, độ bền 30 năm cho công trình dân dụng và nhà xưởng."
            },
            {
                id: 5,
                name: "Tấm Pin Trina Solar N-Type 720W 2 Mặt Kính",
                category: "tam-pin",
                categoryLabel: "Tấm Pin Mặt Trời",
                price: "2.160.000 ₫",
                spec: "Công suất: 720Wp | Bifacial Dual Glass",
                image: "https://images.unsplash.com/photo-1497440001374-f26997328c1b?auto=format&fit=crop&w=600&q=80",
                desc: "Tấm pin năng lượng mặt trời Trina Solar 720W 2 mặt kính chuyên dụng cho các dự án áp mái nhà xưởng, trang trại và hệ thống công suất lớn."
            },
            {
                id: 6,
                name: "Tấm Pin AIKO Solar 650W N-Type ABC",
                category: "tam-pin",
                categoryLabel: "Tấm Pin Mặt Trời",
                price: "2.340.000 ₫",
                spec: "Công suất: 650Wp | All Back Contact",
                image: "https://images.unsplash.com/photo-1548337138-e87d889cc369?auto=format&fit=crop&w=600&q=80",
                desc: "Tấm pin mặt trời AIKO Solar 650W công nghệ ABC chống bóng che cục bộ tối ưu, thẩm mỹ sang trọng cho biệt thự và nhà phố."
            },

            // BIẾN TẦN INVERTER
            {
                id: 7,
                name: "Biến Tần Inverter Hybrid Deye 5kW 1 Pha",
                category: "bien-tan",
                categoryLabel: "Biến Tần Inverter",
                price: "16.500.000 ₫",
                spec: "Model: SUN-5K-SG04LP1 | Hòa lưới có lưu trữ",
                image: "https://images.unsplash.com/photo-1581092160607-ee22621dd758?auto=format&fit=crop&w=600&q=80",
                desc: "Inverter Hybrid Deye 5kW 1 pha tương thích hoàn hảo với pin lưu trữ Lithium Bettenergy, Deye, Pylontech. Hỗ trợ chạy độc lập và bám tải thông minh."
            },
            {
                id: 8,
                name: "Biến Tần Hòa Lưới Growatt 5kW MIN 5000TL-X",
                category: "bien-tan",
                categoryLabel: "Biến Tần Inverter",
                price: "9.200.000 ₫",
                spec: "Công suất: 5kW 1 Pha | 2 MPPT | Hiệu suất 98.4%",
                image: "https://images.unsplash.com/photo-1581092335397-9583fe92d232?auto=format&fit=crop&w=600&q=80",
                desc: "Biến tần hòa lưới Growatt 5kW thiết kế nhỏ gọn, màn hình OLED cảm ứng, theo dõi từ xa qua Wifi ShinePhone ổn định."
            },
            {
                id: 9,
                name: "Biến Tần Hòa Lưới Sofar 7.5kW (7.5KTLM-G2)",
                category: "bien-tan",
                categoryLabel: "Biến Tần Inverter",
                price: "11.000.000 ₫",
                spec: "Công suất: 7.5kW | 2 MPPT | Chuẩn IP65",
                image: "https://images.unsplash.com/photo-1581092580497-e0d23cbdf1dc?auto=format&fit=crop&w=600&q=80",
                desc: "Inverter hòa lưới Sofar 7.5kW hiệu suất 98.2%, tích hợp giám sát thông minh, vận hành êm ái không quạt ồn cho hộ gia đình."
            },
            {
                id: 10,
                name: "Biến Tần Hybrid Luxpower SNA 6kW Phổ Thông",
                category: "bien-tan",
                categoryLabel: "Biến Tần Inverter",
                price: "13.500.000 ₫",
                spec: "Công suất: 6kW | Hòa lưới & Lưu trữ 48V",
                image: "https://images.unsplash.com/photo-1581091226825-a6a2a5aee158?auto=format&fit=crop&w=600&q=80",
                desc: "Biến tần Hybrid Luxpower 6kW được ưa chuộng hàng đầu cho các hệ thống điện mặt trời gia đình có lưu trữ, hỗ trợ ghép song song mở rộng công suất."
            },
            {
                id: 11,
                name: "Biến Tần Công Nghiệp Sungrow 110kW 3 Pha",
                category: "bien-tan",
                categoryLabel: "Biến Tần Inverter",
                price: "86.000.000 ₫",
                spec: "Model: SG110CX | 9 MPPT | Dự án Nhà xưởng",
                image: "https://images.unsplash.com/photo-1592833159155-c62df1b65634?auto=format&fit=crop&w=600&q=80",
                desc: "Inverter hòa lưới 3 pha Sungrow SG110CX công suất 110kW chuyên dụng cho dự án điện mặt trời mái nhà xưởng và doanh nghiệp quy mô lớn."
            },

            // PIN LƯU TRỮ LITHIUM
            {
                id: 12,
                name: "Pin Lưu Trữ Lithium Bettenergy 5kWh (51.2V-100Ah)",
                category: "pin-luu-tru",
                categoryLabel: "Pin Lưu Trữ Lithium",
                price: "22.500.000 ₫",
                spec: "Dung lượng: 5.12kWh | LFP An toàn | BH 10 năm",
                image: "https://images.unsplash.com/photo-1620714223084-8fcacc6dfd8d?auto=format&fit=crop&w=600&q=80",
                desc: "Pin lưu trữ điện mặt trời Bettenergy 5kWh công nghệ Lithium Sắt Photphat (LiFePO4) tuổi thọ trên 6000 chu kỳ sạc xả, giao tiếp tự động với Deye, Luxpower, Growatt."
            },
            {
                id: 13,
                name: "Pin Lưu Trữ Lithium Bettenergy 10.2kWh (51.2V-200Ah)",
                category: "pin-luu-tru",
                categoryLabel: "Pin Lưu Trữ Lithium",
                price: "41.500.000 ₫",
                spec: "Dung lượng: 10.24kWh | Giao tiếp BMS thông minh",
                image: "https://images.unsplash.com/photo-1593941707882-a5bba14938c7?auto=format&fit=crop&w=600&q=80",
                desc: "Bộ lưu trữ Lithium Bettenergy 10kWh đáp ứng thoải mái nhu cầu chạy điều hòa, tủ lạnh, chiếu sáng và thiết bị sinh hoạt xuyên đêm khi mất điện."
            },
            {
                id: 14,
                name: "Pin Lưu Trữ Lithium Bettenergy 16kWh Plus (51.2V-314Ah)",
                category: "pin-luu-tru",
                categoryLabel: "Pin Lưu Trữ Lithium",
                price: "47.000.000 ₫",
                spec: "Dung lượng: 16kWh | Cell LFP 314Ah cao cấp",
                image: "https://images.unsplash.com/photo-1558449028-b53a39d100fc?auto=format&fit=crop&w=600&q=80",
                desc: "Pin lưu trữ dung lượng lớn 16kWh của Bettenergy dành cho biệt thự, văn phòng và hộ gia đình có mức tiêu thụ điện ban đêm cao."
            },
            {
                id: 15,
                name: "Pin Lưu Trữ Lithium Pylontech 16kWh Chính Hãng",
                category: "pin-luu-tru",
                categoryLabel: "Pin Lưu Trữ Lithium",
                price: "56.000.000 ₫",
                spec: "Dung lượng: 16kWh | Chu kỳ sạc > 6000 lần",
                image: "https://images.unsplash.com/photo-1581092162384-8987c1d64718?auto=format&fit=crop&w=600&q=80",
                desc: "Pin lưu trữ Pylontech thương hiệu toàn cầu với hệ thống quản lý BMS độc quyền, độ sâu xả DoD 90% và khả năng mở rộng linh hoạt."
            },

            // COMBO & PHỤ KIỆN
            {
                id: 16,
                name: "Trọn Gói Điện Mặt Trời 5kWp Gia Đình + Tủ Điện ATS",
                category: "combo-phu-kien",
                categoryLabel: "Combo & Phụ Kiện",
                price: "59.000.000 ₫",
                spec: "Trọn gói vật tư + Nhân công lắp đặt hoàn thiện",
                image: "https://images.unsplash.com/photo-1509391366360-2e959784a276?auto=format&fit=crop&w=600&q=80",
                desc: "Gói lắp đặt hoàn chỉnh hệ thống 5kWp cho hộ gia đình gồm tấm pin mặt trời chính hãng, biến tần, tủ điện bảo vệ, khung giàn nhôm và thi công tận nơi."
            }
        ];

        // 2. Danh sách 6 Công trình & Dự án tiêu biểu (Lấy từ thực tế thi công Facebook & EMP.vn)
        const projectsData = [
            {
                id: 101,
                title: "Lắp Đặt Hệ Thống Điện Mặt Trời Hybrid 10kWp + Lưu Trữ 16kWh Tại Đà Nẵng",
                category: "ho-gia-dinh",
                location: "Khu đô thị Hòa Xuân, TP Đà Nẵng",
                capacity: "Công suất: 10kWp + Pin Bettenergy 16kWh",
                image: "https://images.unsplash.com/photo-1508514177221-188b1cf16e9d?auto=format&fit=crop&w=750&q=80",
                desc: "Sử dụng 16 tấm pin Jinko Solar N-Type 620W kết hợp biến tần Hybrid Deye và bộ pin lưu trữ Lithium 16kWh giúp gia chủ tự chủ nguồn điện 24/7, tiết kiệm hơn 4.5 triệu tiền điện mỗi tháng."
            },
            {
                id: 102,
                title: "Công Trình Điện Mặt Trời Hòa Lưới 6kWp Có Lưu Trữ Hộ Gia Đình Xã Đức Phú",
                category: "ho-gia-dinh",
                location: "Xã Đức Phú, TP Đà Nẵng",
                capacity: "Công suất: 6kWp + Lưu trữ 10.2kWh",
                image: "https://images.unsplash.com/photo-1509391366360-2e959784a276?auto=format&fit=crop&w=750&q=80",
                desc: "Thi công trọn gói hệ thống áp mái ngói thẩm mỹ cao, sử dụng tấm pin LONGi Hi-MO X10 650W cùng biến tần Hybrid vận hành tự động, chuyển mạch UPS mượt mà khi cúp điện."
            },
            {
                id: 103,
                title: "Dự Án Điện Mặt Trời Áp Mái Nhà Xưởng Sản Xuất Công Suất 150kWp",
                category: "doanh-nghiep",
                location: "KCN Hòa Cầm, TP Đà Nẵng",
                capacity: "Công suất: 150kWp Hòa lưới 3 Pha",
                image: "https://images.unsplash.com/photo-1613665813446-82a78c468a1d?auto=format&fit=crop&w=750&q=80",
                desc: "Hệ thống sử dụng tấm pin Canadian Solar công suất lớn kết hợp biến tần công nghiệp Sungrow SG110CX, cung cấp nguồn điện xanh trực tiếp cho dây chuyền sản xuất giờ cao điểm."
            },
            {
                id: 104,
                title: "Hệ Thống Điện Mặt Trời 15kWp 3 Pha Cho Khách Sạn & Văn Phòng Ven Biển",
                category: "doanh-nghiep",
                location: "Quận Sơn Trà, TP Đà Nẵng",
                capacity: "Công suất: 15kWp Hòa lưới bám tải",
                image: "https://images.unsplash.com/photo-1497440001374-f26997328c1b?auto=format&fit=crop&w=750&q=80",
                desc: "Giải pháp giảm mạnh chi phí điện điều hòa và thiết bị dịch vụ vào ban ngày, giám sát sản lượng trực tuyến qua ứng dụng điện thoại 24/7."
            },
            {
                id: 105,
                title: "Thi Công Hệ Hybrid 8kWp + Pin Lithium Pylontech Cho Biệt Thự Sân Vườn",
                category: "ho-gia-dinh",
                location: "TP Đà Nẵng",
                capacity: "Công suất: 8kWp + Pin Lithium 10kWh",
                image: "https://images.unsplash.com/photo-1559302504-64aae6ca6b6d?auto=format&fit=crop&w=750&q=80",
                desc: "Thiết kế khung giàn nhôm định hình аноdized chịu bão, đi dây ống ruột gà chống thấm chuẩn kỹ thuật của đội ngũ kỹ sư Hải Vân 68."
            },
            {
                id: 106,
                title: "Dự Án Hệ Thống Lưu Trữ Năng Lượng BESS & Điện Mặt Trời Trang Trại Xanh",
                category: "doanh-nghiep",
                location: "Khu vực Quảng Nam – Đà Nẵng",
                capacity: "Công suất: 50kWp + Lưu trữ BESS 100kWh",
                image: "https://images.unsplash.com/photo-1592833159155-c62df1b65634?auto=format&fit=crop&w=750&q=80",
                desc: "Đáp ứng nguồn điện 3 pha ổn định cho hệ thống tưới tiêu, kho bảo quản nông sản và chiếu sáng an ninh hoàn toàn độc lập với lưới điện."
            }
        ];

        let currentCategory = 'all';
        let currentSearchQuery = '';

        // Hàm hiển thị danh sách sản phẩm (2 cột trên điện thoại, 4 cột trên máy tính, KHÔNG nhãn dán)
        function renderProducts() {
            const grid = document.getElementById('productGrid');
            const filtered = productsData.filter(item => {
                const matchCat = currentCategory === 'all' || item.category === currentCategory;
                const matchSearch = item.name.toLowerCase().includes(currentSearchQuery.toLowerCase()) ||
                                    item.spec.toLowerCase().includes(currentSearchQuery.toLowerCase());
                return matchCat && matchSearch;
            });

            if (filtered.length === 0) {
                grid.innerHTML = `
                    <div class="col-span-2 md:col-span-3 lg:col-span-4 text-center py-10 bg-slate-50 rounded-xl border border-slate-200">
                        <p class="text-sm text-slate-600">Không tìm thấy sản phẩm phù hợp. Vui lòng thử từ khóa khác hoặc liên hệ <strong>0911.310.131</strong>.</p>
                    </div>
                `;
                return;
            }

            grid.innerHTML = filtered.map(product => `
                <div class="fs-box box bg-white rounded-xl border border-slate-200 overflow-hidden flex flex-col justify-between">
                    <div>
                        <div class="box-image aspect-square bg-slate-100 overflow-hidden cursor-pointer" onclick="openProductModal(${product.id})">
                            <img src="${product.image}" 
                                 onerror="this.src='https://placehold.co/500x500/164396/ffffff?text=Hai+Van+68+Solar'"
                                 alt="${product.name}" 
                                 class="w-full h-full object-cover hover:scale-105 transition duration-300">
                        </div>
                        <div class="box-text p-2.5 sm:p-4 pb-2">
                            <div class="text-[10px] sm:text-xs text-slate-400 font-medium mb-1 truncate">${product.categoryLabel}</div>
                            <h3 onclick="openProductModal(${product.id})" class="font-bold text-xs sm:text-sm text-slate-800 hover:text-haivan-blue cursor-pointer line-clamp-2 min-h-[2.4rem] leading-snug">
                                ${product.name}
                            </h3>
                            <p class="text-[11px] text-slate-500 mt-1 truncate hidden sm:block">${product.spec}</p>
                        </div>
                    </div>
                    <div class="px-2.5 sm:px-4 pb-3 pt-1">
                        <div class="font-extrabold text-sm sm:text-base text-haivan-orange mb-2">
                            ${product.price}
                        </div>
                        <div class="grid grid-cols-2 gap-1.5">
                            <button onclick="openProductModal(${product.id})" class="bg-slate-100 hover:bg-slate-200 text-slate-700 font-semibold py-1.5 sm:py-2 rounded-lg text-[11px] sm:text-xs transition">
                                Chi tiết
                            </button>
                            <a href="https://zalo.me/0911310131" target="_blank" class="bg-haivan-blue hover:bg-haivan-darkblue text-white text-center font-semibold py-1.5 sm:py-2 rounded-lg text-[11px] sm:text-xs transition">
                                Báo giá
                            </a>
                        </div>
                    </div>
                </div>
            `).join('');
        }

        // Lọc sản phẩm theo danh mục
        function filterProductsByCategory(category) {
            currentCategory = category;
            document.querySelectorAll('.cat-filter-btn').forEach(btn => {
                if (btn.getAttribute('data-cat-btn') === category) {
                    btn.className = 'cat-filter-btn shrink-0 px-3.5 py-1.5 rounded-lg text-xs font-bold bg-haivan-blue text-white transition';
                } else {
                    btn.className = 'cat-filter-btn shrink-0 px-3.5 py-1.5 rounded-lg text-xs font-bold bg-slate-100 text-slate-700 hover:bg-slate-200 transition';
                }
            });
            const desktopSelect = document.getElementById('desktopSearchCategory');
            if (desktopSelect) desktopSelect.value = category;
            renderProducts();
        }

        function selectCategoryAndScroll(category) {
            filterProductsByCategory(category);
            scrollToSection('san-pham');
        }

        function selectCategoryMobile(category) {
            toggleMobileMenu();
            selectCategoryAndScroll(category);
        }

        function handleSearchInput(query) {
            currentSearchQuery = query;
            renderProducts();
        }

        // Hiển thị Công trình & Dự án (Không nhãn dán đè lên ảnh)
        function renderProjects(filter = 'all') {
            const grid = document.getElementById('projectGrid');
            const filtered = filter === 'all' ? projectsData : projectsData.filter(p => p.category === filter);

            grid.innerHTML = filtered.map(proj => `
                <article class="fs-box bg-white rounded-xl border border-slate-200 overflow-hidden flex flex-col justify-between">
                    <div>
                        <div class="aspect-[16/10] bg-slate-100 overflow-hidden">
                            <img src="${proj.image}" 
                                 onerror="this.src='https://placehold.co/700x450/164396/ffffff?text=Du+An+Hai+Van+68'"
                                 alt="${proj.title}" 
                                 class="w-full h-full object-cover hover:scale-105 transition duration-300">
                        </div>
                        <div class="p-4">
                            <div class="text-xs font-semibold text-haivan-orange mb-1">${proj.capacity}</div>
                            <h3 class="font-bold text-sm sm:text-base text-haivan-blue mb-2 leading-snug">
                                ${proj.title}
                            </h3>
                            <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">
                                ${proj.desc}
                            </p>
                        </div>
                    </div>
                    <div class="px-4 py-3 bg-slate-50 border-t border-slate-100 flex items-center justify-between text-xs text-slate-500">
                        <span><i class="fa-solid fa-location-dot text-haivan-blue mr-1"></i>${proj.location}</span>
                        <a href="tel:0911310131" class="font-bold text-haivan-blue hover:underline">Tư vấn hệ tương tự</a>
                    </div>
                </article>
            `).join('');
        }

        function filterProjects(type) {
            document.querySelectorAll('.proj-filter-btn').forEach(btn => {
                if (btn.getAttribute('data-proj-btn') === type) {
                    btn.className = 'proj-filter-btn shrink-0 px-3 py-1.5 rounded-lg text-xs font-bold bg-haivan-blue text-white';
                } else {
                    btn.className = 'proj-filter-btn shrink-0 px-3 py-1.5 rounded-lg text-xs font-bold bg-white text-slate-700 border border-slate-200';
                }
            });
            renderProjects(type);
        }

        // Công cụ tính toán công suất Điện mặt trời
        function updateSolarCalculator() {
            const bill = document.getElementById('billSelector').value;
            const type = document.getElementById('systemTypeSelector').value;

            const configMap = {
                "2_hybrid": { kw: "Hệ Hybrid 5kWp + Lưu trữ 5kWh", panels: "8 - 9 tấm pin Tier 1", output: "600 – 700 kWh/tháng", area: "~ 22 m²", price: "68.000.000 – 76.000.000 ₫" },
                "2_ongrid": { kw: "Hệ Hòa Lưới 5kWp 1 Pha", panels: "8 - 9 tấm pin Tier 1", output: "600 – 700 kWh/tháng", area: "~ 22 m²", price: "46.000.000 – 53.000.000 ₫" },
                "3_hybrid": { kw: "Hệ Hybrid 6kWp + Lưu trữ 5kWh", panels: "10 tấm pin Tier 1", output: "720 – 850 kWh/tháng", area: "~ 26 m²", price: "75.000.000 – 85.000.000 ₫" },
                "3_ongrid": { kw: "Hệ Hòa Lưới 6kWp 1 Pha", panels: "10 tấm pin Tier 1", output: "720 – 850 kWh/tháng", area: "~ 26 m²", price: "54.000.000 – 62.000.000 ₫" },
                "5_hybrid": { kw: "Hệ Hybrid 8kWp + Lưu trữ 10.2kWh", panels: "14 tấm pin Tier 1", output: "950 – 1.150 kWh/tháng", area: "~ 35 m²", price: "108.000.000 – 122.000.000 ₫" },
                "5_ongrid": { kw: "Hệ Hòa Lưới 8kWp", panels: "14 tấm pin Tier 1", output: "950 – 1.150 kWh/tháng", area: "~ 35 m²", price: "68.000.000 – 78.000.000 ₫" },
                "10_hybrid": { kw: "Hệ Hybrid 12kWp 3 Pha + Lưu trữ 16kWh", panels: "20 tấm pin Tier 1", output: "1.450 – 1.750 kWh/tháng", area: "~ 52 m²", price: "155.000.000 – 175.000.000 ₫" },
                "10_ongrid": { kw: "Hệ Hòa Lưới 12kWp 3 Pha", panels: "20 tấm pin Tier 1", output: "1.450 – 1.750 kWh/tháng", area: "~ 52 m²", price: "98.000.000 – 112.000.000 ₫" },
                "30_hybrid": { kw: "Hệ Hybrid 30kWp 3 Pha + Lưu trữ 50kWh", panels: "50 tấm pin Tier 1", output: "3.600 – 4.200 kWh/tháng", area: "~ 130 m²", price: "390.000.000 – 420.000.000 ₫" },
                "30_ongrid": { kw: "Hệ Hòa Lưới 30kWp 3 Pha Nhà Xưởng", panels: "50 tấm pin Tier 1", output: "3.600 – 4.200 kWh/tháng", area: "~ 130 m²", price: "245.000.000 – 275.000.000 ₫" }
            };

            const data = configMap[`${bill}_${type}`];
            if (data) {
                document.getElementById('calcKw').textContent = data.kw;
                document.getElementById('calcPanels').textContent = data.panels;
                document.getElementById('calcOutput').textContent = data.output;
                document.getElementById('calcArea').textContent = data.area;
                document.getElementById('calcPrice').textContent = data.price;
            }
        }

        // Đóng mở Modal chi tiết sản phẩm
        function openProductModal(id) {
            const product = productsData.find(p => p.id === id);
            if (!product) return;
            document.getElementById('modalTitle').textContent = product.name;
            document.getElementById('modalCategory').textContent = product.categoryLabel;
            document.getElementById('modalPrice').textContent = product.price;
            document.getElementById('modalSpec').textContent = product.spec;
            document.getElementById('modalDesc').textContent = product.desc;
            document.getElementById('modalImage').src = product.image;

            const modal = document.getElementById('productModal');
            modal.classList.remove('hidden');
            modal.classList.add('flex');
        }

        function closeProductModal() {
            const modal = document.getElementById('productModal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        }

        // Đóng mở Modal Shortcode UX Builder
        function openUxShortcodeModal() {
            const modal = document.getElementById('uxShortcodeModal');
            modal.classList.remove('hidden');
            modal.classList.add('flex');
        }

        function closeUxShortcodeModal() {
            const modal = document.getElementById('uxShortcodeModal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        }

        function copyUxShortcode() {
            const textarea = document.getElementById('uxShortcodeText');
            textarea.select();
            document.execCommand('copy');
            const msg = document.getElementById('copyConfirmMsg');
            msg.classList.remove('hidden');
            setTimeout(() => msg.classList.add('hidden'), 3000);
        }

        // Điều khiển Menu Mobile
        function toggleMobileMenu() {
            const drawer = document.getElementById('mobileMenuDrawer');
            const backdrop = document.getElementById('mobileMenuBackdrop');
            const isClosed = drawer.classList.contains('-translate-x-full');
            if (isClosed) {
                drawer.classList.remove('-translate-x-full');
                backdrop.classList.remove('hidden');
            } else {
                drawer.classList.add('-translate-x-full');
                backdrop.classList.add('hidden');
            }
        }

        function scrollToSection(id) {
            const el = document.getElementById(id);
            if (el) el.scrollIntoView({ behavior: 'smooth' });
        }

        // Khởi tạo giao diện khi tải trang
        window.onload = function() {
            renderProducts();
            renderProjects('all');
            updateSolarCalculator();
        };
    </script>
</body>
</html>
