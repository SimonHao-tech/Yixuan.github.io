<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>一轩化工 - 专业污水处理解决方案提供商 | 聚丙烯酰胺供应商</title>
  <!-- 引入外部资源 -->
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/chart.js@4.4.8/dist/chart.umd.min.js"></script>
  
  <!-- Tailwind 配置 -->
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            primary: '#165DFF',
            secondary: '#36CFC9',
            accent: '#FF7D00',
            dark: '#1D2129',
            light: '#F2F3F5'
          },
          fontFamily: {
            sans: ['Inter', 'system-ui', 'sans-serif'],
          },
        },
      }
    }
  </script>
  
  <!-- 自定义工具类 -->
  <style type="text/tailwindcss">
    @layer utilities {
      .content-auto {
        content-visibility: auto;
      }
      .text-shadow {
        text-shadow: 0 2px 4px rgba(0,0,0,0.1);
      }
      .card-hover {
        transition: all 0.3s ease;
      }
      .card-hover:hover {
        transform: translateY(-5px);
        box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
      }
    }
  </style>
  
  <style>
    /* 全局样式 */
    html {
      scroll-behavior: smooth;
    }
    body {
      font-family: 'Inter', system-ui, sans-serif;
    }
    .bg-gradient-primary {
      background: linear-gradient(135deg, #165DFF 0%, #0F48D9 100%);
    }
    .section-padding {
      padding-top: 80px;
      padding-bottom: 80px;
    }
    .section-title {
      position: relative;
      display: inline-block;
    }
    .section-title::after {
      content: '';
      position: absolute;
      bottom: -10px;
      left: 0;
      width: 60px;
      height: 3px;
      background-color: #165DFF;
    }
    .nav-link {
      position: relative;
    }
    .nav-link::after {
      content: '';
      position: absolute;
      bottom: -5px;
      left: 0;
      width: 0;
      height: 2px;
      background-color: #165DFF;
      transition: width 0.3s ease;
    }
    .nav-link:hover::after {
      width: 100%;
    }
    .hero-animation {
      animation: float 6s ease-in-out infinite;
    }
    @keyframes float {
      0% { transform: translateY(0px); }
      50% { transform: translateY(-20px); }
      100% { transform: translateY(0px); }
    }
  </style>
</head>

<body class="text-dark bg-white">
  <!-- 导航栏 -->
  <header id="navbar" class="fixed w-full top-0 z-50 transition-all duration-300 bg-white/95 shadow-sm">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between items-center py-4">
        <!-- Logo -->
        <a href="#" class="flex items-center space-x-2">
          <div class="w-10 h-10 bg-primary rounded-lg flex items-center justify-center">
            <i class="fa fa-tint text-white text-xl"></i>
          </div>
          <span class="text-xl font-bold text-dark">一轩化工</span>
        </a>
        
        <!-- 桌面导航 -->
        <nav class="hidden md:flex items-center space-x-8">
          <a href="#home" class="nav-link text-dark hover:text-primary font-medium">首页</a>
          <a href="#about" class="nav-link text-dark hover:text-primary font-medium">关于我们</a>
          <a href="#products" class="nav-link text-dark hover:text-primary font-medium">产品中心</a>
          <a href="#services" class="nav-link text-dark hover:text-primary font-medium">服务项目</a>
          <a href="#cases" class="nav-link text-dark hover:text-primary font-medium">成功案例</a>
          <a href="#contact" class="nav-link text-dark hover:text-primary font-medium">联系我们</a>
        </nav>
        
        <!-- 联系电话 -->
        <div class="hidden md:flex items-center space-x-1 text-primary">
          <i class="fa fa-phone"></i>
          <span class="font-medium">138-XXXX-XXXX</span>
        </div>
        
        <!-- 移动端菜单按钮 -->
        <button id="menuBtn" class="md:hidden text-dark text-xl">
          <i class="fa fa-bars"></i>
        </button>
      </div>
    </div>
    
    <!-- 移动端导航菜单 -->
    <div id="mobileMenu" class="md:hidden hidden bg-white border-t">
      <div class="container mx-auto px-4 py-3 space-y-3">
        <a href="#home" class="block py-2 text-dark hover:text-primary font-medium">首页</a>
        <a href="#about" class="block py-2 text-dark hover:text-primary font-medium">关于我们</a>
        <a href="#products" class="block py-2 text-dark hover:text-primary font-medium">产品中心</a>
        <a href="#services" class="block py-2 text-dark hover:text-primary font-medium">服务项目</a>
        <a href="#cases" class="block py-2 text-dark hover:text-primary font-medium">成功案例</a>
        <a href="#contact" class="block py-2 text-dark hover:text-primary font-medium">联系我们</a>
        <div class="pt-2 border-t flex items-center space-x-1 text-primary">
          <i class="fa fa-phone"></i>
          <span class="font-medium">138-XXXX-XXXX</span>
        </div>
      </div>
    </div>
  </header>

  <!-- 英雄区域 -->
  <section id="home" class="pt-28 md:pt-0 bg-light overflow-hidden">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex flex-col md:flex-row items-center">
        <div class="md:w-1/2 py-16 md:py-24">
          <h1 class="text-[clamp(2rem,5vw,3.5rem)] font-bold leading-tight text-dark mb-6">
            专业<span class="text-primary">污水处理</span>解决方案<br>
            优质<span class="text-primary">聚丙烯酰胺</span>供应商
          </h1>
          <p class="text-gray-600 text-lg mb-8 max-w-lg">
            一轩化工专注于污水处理领域，提供高品质聚丙烯酰胺产品及定制化污水处理解决方案，服务山西及全国客户。
          </p>
          <div class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-4">
            <a href="#contact" class="bg-primary hover:bg-primary/90 text-white font-medium py-3 px-8 rounded-lg transition-all text-center">
              立即咨询
            </a>
            <a href="#products" class="bg-white hover:bg-gray-50 text-primary border border-primary font-medium py-3 px-8 rounded-lg transition-all text-center">
              查看产品
            </a>
          </div>
          <div class="mt-12 flex items-center space-x-6">
            <div class="flex flex-col">
              <span class="text-3xl font-bold text-primary">10+</span>
              <span class="text-gray-600">行业经验</span>
            </div>
            <div class="flex flex-col">
              <span class="text-3xl font-bold text-primary">500+</span>
              <span class="text-gray-600">成功案例</span>
            </div>
            <div class="flex flex-col">
              <span class="text-3xl font-bold text-primary">24/7</span>
              <span class="text-gray-600">技术支持</span>
            </div>
          </div>
        </div>
        <div class="md:w-1/2 hero-animation">
          <img src="https://picsum.photos/id/1060/600/400" alt="污水处理设备" class="rounded-xl shadow-xl w-full max-w-lg mx-auto">
        </div>
      </div>
    </div>
  </section>

  <!-- 关于我们 -->
  <section id="about" class="section-padding bg-white">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="section-title text-[clamp(1.8rem,3vw,2.5rem)] font-bold text-dark mb-4">关于一轩化工</h2>
        <p class="text-gray-600 max-w-2xl mx-auto">专注污水处理，用心服务每一位客户，致力于成为山西乃至全国领先的水处理化学品供应商</p>
      </div>
      
      <div class="flex flex-col md:flex-row items-center gap-12">
        <div class="md:w-1/2">
          <img src="https://picsum.photos/id/180/600/400" alt="一轩化工厂区" class="rounded-xl shadow-lg w-full h-auto">
        </div>
        <div class="md:w-1/2">
          <h3 class="text-2xl font-bold text-dark mb-6">山西一轩化工科技有限公司</h3>
          <p class="text-gray-600 mb-6">
            一轩化工成立于2015年，位于山西省太原市，是一家专业从事水处理化学品研发、生产、销售及污水处理工程服务的高新技术企业。公司主营聚丙烯酰胺（PAM）系列产品，涵盖阴离子、阳离子、非离子等多种型号，广泛应用于市政污水、工业废水处理、石油开采、造纸、印染等多个领域。
          </p>
          <p class="text-gray-600 mb-8">
            公司拥有先进的生产设备和检测仪器，严格的质量控制体系，确保每一批产品都符合国家标准。我们拥有专业的技术团队，可为客户提供水质分析、产品选型、方案设计、现场调试等一站式服务。
          </p>
          
          <div class="grid grid-cols-2 gap-6 mb-8">
            <div class="flex items-start space-x-3">
              <div class="w-10 h-10 bg-primary/10 rounded-full flex items-center justify-center text-primary mt-1">
                <i class="fa fa-check"></i>
              </div>
              <div>
                <h4 class="font-bold text-dark mb-1">品质保证</h4>
                <p class="text-gray-600 text-sm">严格质量控制</p>
              </div>
            </div>
            <div class="flex items-start space-x-3">
              <div class="w-10 h-10 bg-primary/10 rounded-full flex items-center justify-center text-primary mt-1">
                <i class="fa fa-flask"></i>
              </div>
              <div>
                <h4 class="font-bold text-dark mb-1">技术领先</h4>
                <p class="text-gray-600 text-sm">专业研发团队</p>
              </div>
            </div>
            <div class="flex items-start space-x-3">
              <div class="w-10 h-10 bg-primary/10 rounded-full flex items-center justify-center text-primary mt-1">
                <i class="fa fa-users"></i>
              </div>
              <div>
                <h4 class="font-bold text-dark mb-1">优质服务</h4>
                <p class="text-gray-600 text-sm">24小时技术支持</p>
              </div>
            </div>
            <div class="flex items-start space-x-3">
              <div class="w-10 h-10 bg-primary/10 rounded-full flex items-center justify-center text-primary mt-1">
                <i class="fa fa-map-marker"></i>
              </div>
              <div>
                <h4 class="font-bold text-dark mb-1">立足山西</h4>
                <p class="text-gray-600 text-sm">服务全国客户</p>
              </div>
            </div>
          </div>
          
          <a href="#contact" class="inline-block bg-primary hover:bg-primary/90 text-white font-medium py-3 px-6 rounded-lg transition-all">
            了解更多 <i class="fa fa-arrow-right ml-2"></i>
          </a>
        </div>
      </div>
    </div>
  </section>

  <!-- 产品中心 -->
  <section id="products" class="section-padding bg-light">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="section-title text-[clamp(1.8rem,3vw,2.5rem)] font-bold text-dark mb-4">产品中心</h2>
        <p class="text-gray-600 max-w-2xl mx-auto">高品质聚丙烯酰胺系列产品，满足不同行业污水处理需求</p>
      </div>
      
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        <!-- 产品1 -->
        <div class="bg-white rounded-xl shadow-md p-6 card-hover">
          <div class="w-16 h-16 bg-primary/10 rounded-lg flex items-center justify-center text-primary mb-6">
            <i class="fa fa-tint text-2xl"></i>
          </div>
          <h3 class="text-xl font-bold text-dark mb-3">阴离子聚丙烯酰胺</h3>
          <p class="text-gray-600 mb-4">
            分子量800-2200万，主要用于工业废水处理、污水处理厂污泥脱水、饮用水净化等。
          </p>
          <div class="mb-6">
            <h4 class="font-medium text-dark mb-2">应用领域：</h4>
            <div class="flex flex-wrap gap-2">
              <span class="bg-gray-100 text-gray-700 text-sm py-1 px-3 rounded-full">市政污水处理</span>
              <span class="bg-gray-100 text-gray-700 text-sm py-1 px-3 rounded-full">工业废水处理</span>
              <span class="bg-gray-100 text-gray-700 text-sm py-1 px-3 rounded-full">污泥脱水</span>
            </div>
          </div>
          <a href="#contact" class="text-primary font-medium hover:text-primary/80 flex items-center">
            咨询详情 <i class="fa fa-angle-right ml-2"></i>
          </a>
        </div>
        
        <!-- 产品2 -->
        <div class="bg-white rounded-xl shadow-md p-6 card-hover">
          <div class="w-16 h-16 bg-primary/10 rounded-lg flex items-center justify-center text-primary mb-6">
            <i class="fa fa-tint text-2xl"></i>
          </div>
          <h3 class="text-xl font-bold text-dark mb-3">阳离子聚丙烯酰胺</h3>
          <p class="text-gray-600 mb-4">
            离子度10-80%，主要用于造纸废水处理、印染废水处理、啤酒厂废水处理等有机废水处理。
          </p>
          <div class="mb-6">
            <h4 class="font-medium text-dark mb-2">应用领域：</h4>
            <div class="flex flex-wrap gap-2">
              <span class="bg-gray-100 text-gray-700 text-sm py-1 px-3 rounded-full">造纸废水</span>
              <span class="bg-gray-100 text-gray-700 text-sm py-1 px-3 rounded-full">印染废水</span>
              <span class="bg-gray-100 text-gray-700 text-sm py-1 px-3 rounded-full">食品加工废水</span>
            </div>
          </div>
          <a href="#contact" class="text-primary font-medium hover:text-primary/80 flex items-center">
            咨询详情 <i class="fa fa-angle-right ml-2"></i>
          </a>
        </div>
        
        <!-- 产品3 -->
        <div class="bg-white rounded-xl shadow-md p-6 card-hover">
          <div class="w-16 h-16 bg-primary/10 rounded-lg flex items-center justify-center text-primary mb-6">
            <i class="fa fa-tint text-2xl"></i>
          </div>
          <h3 class="text-xl font-bold text-dark mb-3">非离子聚丙烯酰胺</h3>
          <p class="text-gray-600 mb-4">
            主要用于水处理助凝剂、纺织工业助剂、土壤保湿剂、油田化学剂等多种用途。
          </p>
          <div class="mb-6">
            <h4 class="font-medium text-dark mb-2">应用领域：</h4>
            <div class="flex flex-wrap gap-2">
              <span class="bg-gray-100 text-gray-700 text-sm py-1 px-3 rounded-full">水处理助凝</span>
              <span class="bg-gray-100 text-gray-700 text-sm py-1 px-3 rounded-full">纺织助剂</span>
              <span class="bg-gray-100 text-gray-700 text-sm py-1 px-3 rounded-full">油田化学</span>
            </div>
          </div>
          <a href="#contact" class="text-primary font-medium hover:text-primary/80 flex items-center">
            咨询详情 <i class="fa fa-angle-right ml-2"></i>
          </a>
        </div>
        
        <!-- 产品4 -->
        <div class="bg-white rounded-xl shadow-md p-6 card-hover">
          <div class="w-16 h-16 bg-primary/10 rounded-lg flex items-center justify-center text-primary mb-6">
            <i class="fa fa-tint text-2xl"></i>
          </div>
          <h3 class="text-xl font-bold text-dark mb-3">两性离子聚丙烯酰胺</h3>
          <p class="text-gray-600 mb-4">
            兼具阴、阳离子特性，适用于复杂水质处理，在油田、造纸、印染等行业有广泛应用。
          </p>
          <div class="mb-6">
            <h4 class="font-medium text-dark mb-2">应用领域：</h4>
            <div class="flex flex-wrap gap-2">
              <span class="bg-gray-100 text-gray-700 text-sm py-1 px-3 rounded-full">复杂水质处理</span>
              <span class="bg-gray-100 text-gray-700 text-sm py-1 px-3 rounded-full">油田开采</span>
              <span class="bg-gray-100 text-gray-700 text-sm py-1 px-3 rounded-full">造纸行业</span>
            </div>
          </div>
          <a href="#contact" class="text-primary font-medium hover:text-primary/80 flex items-center">
            咨询详情 <i class="fa fa-angle-right ml-2"></i>
          </a>
        </div>
        
        <!-- 产品5 -->
        <div class="bg-white rounded-xl shadow-md p-6 card-hover">
          <div class="w-16 h-16 bg-primary/10 rounded-lg flex items-center justify-center text-primary mb-6">
            <i class="fa fa-tint text-2xl"></i>
          </div>
          <h3 class="text-xl font-bold text-dark mb-3">聚合氯化铝</h3>
          <p class="text-gray-600 mb-4">
            高效净水剂，广泛应用于饮用水、工业用水和污水处理等领域，具有混凝效果好、用量少等特点。
          </p>
          <div class="mb-6">
            <h4 class="font-medium text-dark mb-2">应用领域：</h4>
            <div class="flex flex-wrap gap-2">
              <span class="bg-gray-100 text-gray-700 text-sm py-1 px-3 rounded-full">饮用水净化</span>
              <span class="bg-gray-100 text-gray-700 text-sm py-1 px-3 rounded-full">工业用水处理</span>
              <span class="bg-gray-100 text-gray-700 text-sm py-1 px-3 rounded-full">污水处理</span>
            </div>
          </div>
          <a href="#contact" class="text-primary font-medium hover:text-primary/80 flex items-center">
            咨询详情 <i class="fa fa-angle-right ml-2"></i>
          </a>
        </div>
        
        <!-- 产品6 -->
        <div class="bg-white rounded-xl shadow-md p-6 card-hover">
          <div class="w-16 h-16 bg-primary/10 rounded-lg flex items-center justify-center text-primary mb-6">
            <i class="fa fa-tint text-2xl"></i>
          </div>
          <h3 class="text-xl font-bold text-dark mb-3">水处理专用药剂</h3>
          <p class="text-gray-600 mb-4">
            定制化水处理药剂，包括消泡剂、脱色剂、缓蚀阻垢剂等，满足不同客户的特殊处理需求。
          </p>
          <div class="mb-6">
            <h4 class="font-medium text-dark mb-2">应用领域：</h4>
            <div class="flex flex-wrap gap-2">
              <span class="bg-gray-100 text-gray-700 text-sm py-1 px-3 rounded-full">工业循环水</span>
              <span class="bg-gray-100 text-gray-700 text-sm py-1 px-3 rounded-full">废水脱色</span>
              <span class="bg-gray-100 text-gray-700 text-sm py-1 px-3 rounded-full">消泡处理</span>
            </div>
          </div>
          <a href="#contact" class="text-primary font-medium hover:text-primary/80 flex items-center">
            咨询详情 <i class="fa fa-angle-right ml-2"></i>
          </a>
        </div>
      </div>
    </div>
  </section>

  <!-- 服务项目 -->
  <section id="services" class="section-padding bg-white">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="section-title text-[clamp(1.8rem,3vw,2.5rem)] font-bold text-dark mb-4">服务项目</h2>
        <p class="text-gray-600 max-w-2xl mx-auto">提供全方位污水处理解决方案，从技术咨询到现场调试的一站式服务</p>
      </div>
      
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        <!-- 服务1 -->
        <div class="bg-light rounded-xl p-8 card-hover">
          <div class="w-14 h-14 bg-primary/10 rounded-full flex items-center justify-center text-primary mb-6">
            <i class="fa fa-line-chart text-2xl"></i>
          </div>
          <h3 class="text-xl font-bold text-dark mb-4">水质分析检测</h3>
          <p class="text-gray-600">
            专业的水质检测团队，提供全面的水质分析服务，为客户精准判断水质状况，制定针对性处理方案。
          </p>
        </div>
        
        <!-- 服务2 -->
        <div class="bg-light rounded-xl p-8 card-hover">
          <div class="w-14 h-14 bg-primary/10 rounded-full flex items-center justify-center text-primary mb-6">
            <i class="fa fa-cogs text-2xl"></i>
          </div>
          <h3 class="text-xl font-bold text-dark mb-4">产品选型推荐</h3>
          <p class="text-gray-600">
            根据客户水质情况和处理要求，提供最适合的聚丙烯酰胺产品型号推荐，确保处理效果和成本优化。
          </p>
        </div>
        
        <!-- 服务3 -->
        <div class="bg-light rounded-xl p-8 card-hover">
          <div class="w-14 h-14 bg-primary/10 rounded-full flex items-center justify-center text-primary mb-6">
            <i class="fa fa-file-text text-2xl"></i>
          </div>
          <h3 class="text-xl font-bold text-dark mb-4">处理方案设计</h3>
          <p class="text-gray-600">
            定制化污水处理方案设计，包括药剂投加量、处理工艺优化等，帮助客户实现高效、经济的污水处理。
          </p>
        </div>
        
        <!-- 服务4 -->
        <div class="bg-light rounded-xl p-8 card-hover">
          <div class="w-14 h-14 bg-primary/10 rounded-full flex items-center justify-center text-primary mb-6">
            <i class="fa fa-wrench text-2xl"></i>
          </div>
          <h3 class="text-xl font-bold text-dark mb-4">现场技术调试</h3>
          <p class="text-gray-600">
            专业技术人员现场指导药剂投加和设备调试，确保处理效果达到预期，解决实际运行中的技术问题。
          </p>
        </div>
        
        <!-- 服务5 -->
        <div class="bg-light rounded-xl p-8 card-hover">
          <div class="w-14 h-14 bg-primary/10 rounded-full flex items-center justify-center text-primary mb-6">
            <i class="fa fa-truck text-2xl"></i>
          </div>
          <h3 class="text-xl font-bold text-dark mb-4">快速物流配送</h3>
          <p class="text-gray-600">
            覆盖山西及全国的物流配送网络，确保产品及时送达，满足客户生产需求，提供便捷的供货服务。
          </p>
        </div>
        
        <!-- 服务6 -->
        <div class="bg-light rounded-xl p-8 card-hover">
          <div class="w-14 h-14 bg-primary/10 rounded-full flex items-center justify-center text-primary mb-6">
            <i class="fa fa-headphones text-2xl"></i>
          </div>
          <h3 class="text-xl font-bold text-dark mb-4">24小时技术支持</h3>
          <p class="text-gray-600">
            全天候技术咨询服务，随时解答客户在产品使用和污水处理过程中遇到的问题，提供专业解决方案。
          </p>
        </div>
      </div>
    </div>
  </section>

  <!-- 成功案例 -->
  <section id="cases" class="section-padding bg-light">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="section-title text-[clamp(1.8rem,3vw,2.5rem)] font-bold text-dark mb-4">成功案例</h2>
        <p class="text-gray-600 max-w-2xl mx-auto">多年行业经验，服务众多客户，积累了丰富的成功案例</p>
      </div>
      
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <!-- 案例1 -->
        <div class="bg-white rounded-xl shadow-md overflow-hidden card-hover">
          <div class="h-60 overflow-hidden">
            <img src="https://picsum.photos/id/1047/600/400" alt="化工废水处理案例" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
          </div>
          <div class="p-6">
            <div class="flex items-center mb-4">
              <span class="bg-primary/10 text-primary text-sm py-1 px-3 rounded-full">化工废水处理</span>
            </div>
            <h3 class="text-xl font-bold text-dark mb-3">山西某化工企业废水处理项目</h3>
            <p class="text-gray-600 mb-4">
              为山西某大型化工企业提供阴离子聚丙烯酰胺产品及污水处理解决方案，处理水量10000m³/d，COD去除率达到92%以上，出水水质达到国家一级排放标准。
            </p>
            <div class="flex justify-between items-center">
              <span class="text-gray-500 text-sm">合作时间：2022年</span>
              <a href="#contact" class="text-primary font-medium hover:text-primary/80">
                查看详情 <i class="fa fa-arrow-right ml-1"></i>
              </a>
            </div>
          </div>
        </div>
        
        <!-- 案例2 -->
        <div class="bg-white rounded-xl shadow-md overflow-hidden card-hover">
          <div class="h-60 overflow-hidden">
            <img src="https://picsum.photos/id/1059/600/400" alt="市政污水处理案例" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
          </div>
          <div class="p-6">
            <div class="flex items-center mb-4">
              <span class="bg-primary/10 text-primary text-sm py-1 px-3 rounded-full">市政污水处理</span>
            </div>
            <h3 class="text-xl font-bold text-dark mb-3">太原某污水处理厂污泥脱水项目</h3>
            <p class="text-gray-600 mb-4">
              为太原某污水处理厂提供阳离子聚丙烯酰胺产品，用于污泥脱水处理，污泥含水率从98%降至65%以下，大大降低了污泥处置成本，提高了处理效率。
            </p>
            <div class="flex justify-between items-center">
              <span class="text-gray-500 text-sm">合作时间：2021年</span>
              <a href="#contact" class="text-primary font-medium hover:text-primary/80">
                查看详情 <i class="fa fa-arrow-right ml-1"></i>
              </a>
            </div>
          </div>
        </div>
        
        <!-- 案例3 -->
        <div class="bg-white rounded-xl shadow-md overflow-hidden card-hover">
          <div class="h-60 overflow-hidden">
            <img src="https://picsum.photos/id/1054/600/400" alt="印染废水处理案例" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
          </div>
          <div class="p-6">
            <div class="flex items-center mb-4">
              <span class="bg-primary/10 text-primary text-sm py-1 px-3 rounded-full">印染废水处理</span>
            </div>
            <h3 class="text-xl font-bold text-dark mb-3">晋中某印染厂废水处理项目</h3>
            <p class="text-gray-600 mb-4">
              为晋中某印染厂提供两性离子聚丙烯酰胺及脱色剂产品，处理印染废水5000m³/d，色度去除率达到95%，COD去除率88%，实现水资源循环利用。
            </p>
            <div class="flex justify-between items-center">
              <span class="text-gray-500 text-sm">合作时间：2023年</span>
              <a href="#contact" class="text-primary font-medium hover:text-primary/80">
                查看详情 <i class="fa fa-arrow-right ml-1"></i>
              </a>
            </div>
          </div>
        </div>
        
        <!-- 案例4 -->
        <div class="bg-white rounded-xl shadow-md overflow-hidden card-hover">
          <div class="h-60 overflow-hidden">
            <img src="https://picsum.photos/id/1058/600/400" alt="造纸废水处理案例" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
          </div>
          <div class="p-6">
            <div class="flex items-center mb-4">
              <span class="bg-primary/10 text-primary text-sm py-1 px-3 rounded-full">造纸废水处理</span>
            </div>
            <h3 class="text-xl font-bold text-dark mb-3">运城某造纸厂废水处理项目</h3>
            <p class="text-gray-600 mb-4">
              为运城某造纸厂提供阳离子聚丙烯酰胺产品，用于造纸中段废水处理和污泥脱水，处理水量8000m³/d，SS去除率96%，实现废水达标排放和污泥资源化利用。
            </p>
            <div class="flex justify-between items-center">
              <span class="text-gray-500 text-sm">合作时间：2022年</span>
              <a href="#contact" class="text-primary font-medium hover:text-primary/80">
                查看详情 <i class="fa fa-arrow-right ml-1"></i>
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- 数据统计 -->
  <section class="bg-gradient-primary py-16">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid grid-cols-2 md:grid-cols-4 gap-8 text-center">
        <div class="text-white">
          <div class="text-4xl md:text-5xl font-bold mb-2 counter" data-target="10">0</div>
          <p class="text-white/80">年行业经验</p>
        </div>
        <div class="text-white">
          <div class="text-4xl md:text-5xl font-bold mb-2 counter" data-target="500">0</div>
          <p class="text-white/80">成功案例</p>
        </div>
        <div class="text-white">
          <div class="text-4xl md:text-5xl font-bold mb-2 counter" data-target="300">0</div>
          <p class="text-white/80">合作客户</p>
        </div>
        <div class="text-white">
          <div class="text-4xl md:text-5xl font-bold mb-2 counter" data-target="24">0</div>
          <p class="text-white/80">小时技术支持</p>
        </div>
      </div>
    </div>
  </section>

  <!-- 联系我们 -->
  <section id="contact" class="section-padding bg-white">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="section-title text-[clamp(1.8rem,3vw,2.5rem)] font-bold text-dark mb-4">联系我们</h2>
        <p class="text-gray-600 max-w-2xl mx-auto">无论您有任何疑问或需求，欢迎随时联系我们，我们将竭诚为您服务</p>
      </div>
      
      <div class="flex flex-col lg:flex-row gap-12">
        <div class="lg:w-1/2">
          <div class="bg-light rounded-xl p-8">
            <h3 class="text-2xl font-bold text-dark mb-6">联系方式</h3>
            <div class="space-y-6">
              <div class="flex items-start space-x-4">
                <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center text-primary mt-1">
                  <i class="fa fa-map-marker"></i>
                </div>
                <div>
                  <h4 class="font-bold text-dark mb-1">公司地址</h4>
                  <p class="text-gray-600">山西省太原市晋源区化工园区8号</p>
                </div>
              </div>
              
              <div class="flex items-start space-x-4">
                <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center text-primary mt-1">
                  <i class="fa fa-phone"></i>
                </div>
                <div>
                  <h4 class="font-bold text-dark mb-1">联系电话</h4>
                  <p class="text-gray-600">郝经理：138-XXXX-XXXX</p>
                  <p class="text-gray-600">固话：0351-XXXXXXX</p>
                </div>
              </div>
              
              <div class="flex items-start space-x-4">
                <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center text-primary mt-1">
                  <i class="fa fa-envelope"></i>
                </div>
                <div>
                  <h4 class="font-bold text-dark mb-1">电子邮箱</h4>
                  <p class="text-gray-600">yixuanhuagong@163.com</p>
                </div>
              </div>
              
              <div class="flex items-start space-x-4">
                <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center text-primary mt-1">
                  <i class="fa fa-clock-o"></i>
                </div>
                <div>
                  <h4 class="font-bold text-dark mb-1">工作时间</h4>
                  <p class="text-gray-600">周一至周五：8:00-18:00</p>
                  <p class="text-gray-600">周六：9:00-16:00（节假日除外）</p>
                </div>
              </div>
            </div>
            
            <div class="mt-8">
              <h4 class="font-bold text-dark mb-4">关注我们</h4>
              <div class="flex space-x-4">
                <a href="#" class="w-10 h-10 bg-primary/10 rounded-full flex items-center justify-center text-primary hover:bg-primary hover:text-white transition-all">
                  <i class="fa fa-weixin"></i>
                </a>
                <a href="#" class="w-10 h-10 bg-primary/10 rounded-full flex items-center justify-center text-primary hover:bg-primary hover:text-white transition-all">
                  <i class="fa fa-weibo"></i>
                </a>
                <a href="#" class="w-10 h-10 bg-primary/10 rounded-full flex items-center justify-center text-primary hover:bg-primary hover:text-white transition-all">
                  <i class="fa fa-qq"></i>
                </a>
                <a href="#" class="w-10 h-10 bg-primary/10 rounded-full flex items-center justify-center text-primary hover:bg-primary hover:text-white transition-all">
                  <i class="fa fa-linkedin"></i>
                </a>
              </div>
            </div>
          </div>
        </div>
        
        <div class="lg:w-1/2">
          <div class="bg-light rounded-xl p-8">
            <h3 class="text-2xl font-bold text-dark mb-6">在线咨询</h3>
            <form>
              <div class="grid grid-cols-1 sm:grid-cols-2 gap-6 mb-6">
                <div>
                  <label for="name" class="block text-gray-700 font-medium mb-2">您的姓名</label>
                  <input type="text" id="name" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent" placeholder="请输入您的姓名">
                </div>
                <div>
                  <label for="phone" class="block text-gray-700 font-medium mb-2">联系电话</label>
                  <input type="tel" id="phone" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent" placeholder="请输入您的联系电话">
                </div>
              </div>
              
              <div class="mb-6">
                <label for="company" class="block text-gray-700 font-medium mb-2">公司名称</label>
                <input type="text" id="company" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent" placeholder="请输入您的公司名称">
              </div>
              
              <div class="mb-6">
                <label for="product" class="block text-gray-700 font-medium mb-2">咨询产品/服务</label>
                <select id="product" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent">
                  <option value="">请选择咨询产品/服务</option>
                  <option value="阴离子聚丙烯酰胺">阴离子聚丙烯酰胺</option>
                  <option value="阳离子聚丙烯酰胺">阳离子聚丙烯酰胺</option>
                  <option value="非离子聚丙烯酰胺">非离子聚丙烯酰胺</option>
                  <option value="两性离子聚丙烯酰胺">两性离子聚丙烯酰胺</option>
                  <option value="聚合氯化铝">聚合氯化铝</option>
                  <option value="水处理方案设计">水处理方案设计</option>
                  <option value="其他产品/服务">其他产品/服务</option>
                </select>
              </div>
              
              <div class="mb-6">
                <label for="message" class="block text-gray-700 font-medium mb-2">留言内容</label>
                <textarea id="message" rows="4" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent" placeholder="请输入您的留言内容"></textarea>
              </div>
              
              <button type="submit" class="w-full bg-primary hover:bg-primary/90 text-white font-medium py-3 px-6 rounded-lg transition-all">
                提交咨询 <i class="fa fa-paper-plane ml-2"></i>
              </button>
            </form>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- 页脚 -->
  <footer class="bg-dark text-white pt-16 pb-8">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-12 mb-12">
        <div>
          <div class="flex items-center space-x-2 mb-6">
            <div class="w-10 h-10 bg-white rounded-lg flex items-center justify-center">
              <i class="fa fa-tint text-primary text-xl"></i>
            </div>
            <span class="text-xl font-bold">一轩化工</span>
          </div>
          <p class="text-gray-400 mb-6">
            专注于污水处理领域，提供高品质聚丙烯酰胺产品及定制化污水处理解决方案，服务山西及全国客户。
          </p>
          <div class="flex space-x-4">
            <a href="#" class="w-10 h-10 bg-gray-800 rounded-full flex items-center justify-center text-gray-400 hover:bg-primary hover:text-white transition-all">
              <i class="fa fa-weixin"></i>
            </a>
            <a href="#" class="w-10 h-10 bg-gray-800 rounded-full flex items-center justify-center text-gray-400 hover:bg-primary hover:text-white transition-all">
              <i class="fa fa-weibo"></i>
            </a>
            <a href="#" class="w-10 h-10 bg-gray-800 rounded-full flex items-center justify-center text-gray-400 hover:bg-primary hover:text-white transition-all">
              <i class="fa fa-qq"></i>
            </a>
            <a href="#" class="w-10 h-10 bg-gray-800 rounded-full flex items-center justify-center text-gray-400 hover:bg-primary hover:text-white transition-all">
              <i class="fa fa-linkedin"></i>
            </a>
          </div>
        </div>
        
        <div>
          <h4 class="text-lg font-bold mb-6">快速链接</h4>
          <ul class="space-y-3">
            <li><a href="#home" class="text-gray-400 hover:text-white transition-colors">首页</a></li>
            <li><a href="#about" class="text-gray-400 hover:text-white transition-colors">关于我们</a></li>
            <li><a href="#products" class="text-gray-400 hover:text-white transition-colors">产品中心</a></li>
            <li><a href="#services" class="text-gray-400 hover:text-white transition-colors">服务项目</a></li>
            <li><a href="#cases" class="text-gray-400 hover:text-white transition-colors">成功案例</a></li>
            <li><a href="#contact" class="text-gray-400 hover:text-white transition-colors">联系我们</a></li>
          </ul>
        </div>
        
        <div>
          <h4 class="text-lg font-bold mb-6">产品系列</h4>
          <ul class="space-y-3">
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors">阴离子聚丙烯酰胺</a></li>
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors">阳离子聚丙烯酰胺</a></li>
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors">非离子聚丙烯酰胺</a></li>
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors">两性离子聚丙烯酰胺</a></li>
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors">聚合氯化铝</a></li>
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors">水处理专用药剂</a></li>
          </ul>
        </div>
        
        <div>
          <h4 class="text-lg font-bold mb-6">联系信息</h4>
          <ul class="space-y-3">
            <li class="flex items-start space-x-3">
              <i class="fa fa-map-marker text-primary mt-1"></i>
              <span class="text-gray-400">山西省太原市晋源区化工园区8号</span>
            </li>
            <li class="flex items-start space-x-3">
              <i class="fa fa-phone text-primary mt-1"></i>
              <span class="text-gray-400">郝经理：138-XXXX-XXXX</span>
            </li>
            <li class="flex items-start space-x-3">
              <i class="fa fa-phone text-primary mt-1"></i>
              <span class="text-gray-400">固话：0351-XXXXXXX</span>
            </li>
            <li class="flex items-start space-x-3">
              <i class="fa fa-envelope text-primary mt-1"></i>
              <span class="text-gray-400">yixuanhuagong@163.com</span>
            </li>
            <li class="flex items-start space-x-3">
              <i class="fa fa-clock-o text-primary mt-1"></i>
              <span class="text-gray-400">周一至周五：8:00-18:00</span>
            </li>
          </ul>
        </div>
      </div>
      
      <div class="border-t border-gray-800 pt-8">
        <div class="flex flex-col md:flex-row justify-between items-center">
          <p class="text-gray-500 text-sm mb-4 md:mb-0">
            © 2025 山西一轩化工科技有限公司 版权所有 | 晋ICP备XXXXXXXX号
          </p>
          <div class="flex space-x-6">
            <a href="#" class="text-gray-500 hover:text-gray-400 text-sm">隐私政策</a>
            <a href="#" class="text-gray-500 hover:text-gray-400 text-sm">服务条款</a>
            <a href="#" class="text-gray-500 hover:text-gray-400 text-sm">网站地图</a>
          </div>
        </div>
      </div>
    </div>
  </footer>

  <!-- 回到顶部按钮 -->
  <button id="backToTop" class="fixed bottom-8 right-8 w-12 h-12 bg-primary rounded-full flex items-center justify-center text-white shadow-lg opacity-0 invisible transition-all duration-300 z-50">
    <i class="fa fa-arrow-up"></i>
  </button>

  <!-- JavaScript -->
  <script>
    // 移动端菜单切换
    const menuBtn = document.getElementById('menuBtn');
    const mobileMenu = document.getElementById('mobileMenu');
    
    menuBtn.addEventListener('click', () => {
      mobileMenu.classList.toggle('hidden');
      if (mobileMenu.classList.contains('hidden')) {
        menuBtn.innerHTML = '<i class="fa fa-bars"></i>';
      } else {
        menuBtn.innerHTML = '<i class="fa fa-times"></i>';
      }
    });
    
    // 导航栏滚动效果
    const navbar = document.getElementById('navbar');
    const backToTop = document.getElementById('backToTop');
    
    window.addEventListener('scroll', () => {
      if (window.scrollY > 100) {
        navbar.classList.add('shadow-md');
        navbar.classList.remove('py-4');
        navbar.classList.add('py-2');
        
        backToTop.classList.remove('opacity-0', 'invisible');
        backToTop.classList.add('opacity-100', 'visible');
      } else {
        navbar.classList.remove('shadow-md');
        navbar.classList.remove('py-2');
        navbar.classList.add('py-4');
        
        backToTop.classList.add('opacity-0', 'invisible');
        backToTop.classList.remove('opacity-100', 'visible');
      }
    });
    
    // 回到顶部功能
    backToTop.addEventListener('click', () => {
      window.scrollTo({
        top: 0,
        behavior: 'smooth'
      });
    });
    
    // 数字计数动画
    const counters = document.querySelectorAll('.counter');
    let counted = false;
    
    function startCounting() {
      counters.forEach(counter => {
        const target = parseInt(counter.getAttribute('data-target'));
        const duration = 2000; // 动画持续时间（毫秒）
        const stepTime = 20; // 每步时间（毫秒）
        const totalSteps = duration / stepTime;
        const stepSize = target / totalSteps;
        let current = 0;
        
        const timer = setInterval(() => {
          current += stepSize;
          counter.innerText = Math.ceil(current);
          if (current >= target) {
            counter.innerText = target;
            clearInterval(timer);
          }
        }, stepTime);
      });
    }
    
    // 监听滚动，当统计区域进入视图时开始计数
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting && !counted) {
          startCounting();
          counted = true;
        }
      });
    }, { threshold: 0.5 });
    
    if (counters.length > 0) {
      observer.observe(counters[0].parentElement.parentElement);
    }
    
    // 平滑滚动
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        e.preventDefault();
        
        // 关闭移动端菜单
        if (!mobileMenu.classList.contains('hidden')) {
          mobileMenu.classList.add('hidden');
          menuBtn.innerHTML = '<i class="fa fa-bars"></i>';
        }
        
        const targetId = this.getAttribute('href');
        if (targetId === '#') return;
        
        const targetElement = document.querySelector(targetId);
        if (targetElement) {
          const navbarHeight = navbar.offsetHeight;
          const targetPosition = targetElement.getBoundingClientRect().top + window.pageYOffset - navbarHeight;
          
          window.scrollTo({
            top: targetPosition,
            behavior: 'smooth'
          });
        }
      });
    });
  </script>
</body>
</html>
