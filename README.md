 <!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>TRỊNH HÀ NINH</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
<style>
:root{
    --primary:#2ecc71;
    --red:#e74c3c;
    --bg:#f8f9fa;
    --border:#ddd;
    --light:#7f8c8d;}
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, Helvetica, sans-serif;}
body{
    background:var(--bg);}
header{
    background:#fff;
    border-bottom:1px solid var(--border);
    padding:20px 5%;}
.header-top{
    display:flex;
    justify-content:space-between;
    align-items:flex-start;}
.brand{
    display:flex;
    align-items:center;
    gap:10px;}
.brand-text{
    display:grid;
    grid-template-columns:auto auto;
    grid-template-rows:auto auto;
    column-gap:10px;}
.brand-top{
    grid-column:1/3;
    font-size:12px;
    color:#0099FF;
    font-weight:bold;}
.brand-main{
    grid-column:1/3;
    font-size:30px;
    font-weight:900;
    color:#FF9966}
.brand-bottom-row{
    grid-column:2;
    display:flex;
    align-items:center;
    gap:6px;
    justify-self:end;}
.brand-bottom{
    color:red;
    font-weight:bold;}
.logo{
    width:25px;}
.date-vertical{
    writing-mode:vertical-rl;
    transform:rotate(180deg);
    font-size:12px;
    color:var(--light);
    margin-left:10px;}
.auth a{
    margin-left:15px;
    font-weight:bold;
    text-decoration:none;
    color:#000;}
.banner{
    width:100%;
    height:220px;
    background:url("istockphoto-2148264573-612x612.jpg") no-repeat center center;
    background-size:cover;
    display:flex;
    align-items:center;
    justify-content:center;
    position:relative;
    margin-top:15px;}
.banner::after{
    content:"";
    position:absolute;
    inset:0;
    background:rgba(0,0,0,0.4);}
.banner-content{
    position:relative;
    text-align:center;
    color:#fff;
    z-index:1;}
.banner-content h1{
    font-size:28px;
    font-weight:bold;
    margin-bottom:8px;}
.banner-content p{
    font-size:16px;
    letter-spacing:1px;}
    nav{
    margin-top:15px;
    display:flex;
    justify-content:space-between;
    gap:20px;
    overflow-x:auto;}
nav a{
    font-weight:700;
    color:#666;
    text-decoration:none;
    white-space:nowrap;}
nav a:hover{
    color:var(--primary);}
main{
    max-width:1100px;
    margin:auto;
    padding:40px 5%;
    background:#ffe6ee;}
.search-bar{
    background:#fff;
    border:1px solid var(--border);
    border-radius:30px;
    height:50px;
    display:flex;
    align-items:center;
    padding:0 20px;
    margin-bottom:30px;}
.search-bar input{
    flex:1;
    border:none;
    outline:none;
    font-size:16px;
    padding:0 10px;}
.hero{
    display:flex;
    flex-direction:column;
    align-items:center;
    gap:25px;
    margin-bottom:40px;}
.chart-box{
    background:#fff;
    padding:25px;
    border-radius:15px;
    width:100%;
    max-width:800px;
    box-shadow:0 5px 15px rgba(0,0,0,0.05);}
.line{
    fill:none;
    stroke:var(--primary);
    stroke-width:3;
    stroke-dasharray:1000;
    stroke-dashoffset:1000;
    animation:draw 3s forwards;}
@keyframes draw{
    to{stroke-dashoffset:0;}}
.marquee-text{
    width:100%;
    font-size:clamp(24px,5vw,40px);
    font-weight:900;
    text-transform:uppercase;
    overflow:hidden;
    white-space:nowrap;
    border-top:2px solid var(--primary);
    padding-top:15px;}
.marquee-content{
    display:inline-block;
    padding-left:100%;
    animation:marquee 15s linear infinite;}
@keyframes marquee{
    100%{transform:translateX(-100%);}}
.section-title{
    border-left:5px solid var(--primary);
    padding-left:15px;
    margin:30px 0 20px;
    font-size:22px;}
.stock-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
    gap:20px;
    margin-bottom:40px;}
.stock-card{
    background:#fff;
    border:1px solid var(--border);
    border-radius:12px;
    padding:25px;
    text-align:center;
    transition:0.3s;}
.stock-card:hover{
    transform:translateY(-5px);
    box-shadow:0 10px 20px rgba(0,0,0,0.1);}
.stock-card h3{
    color:black;
    font-size:24px;}

.stock-card h5{
    color:var(--light);
    margin-top:6px;}
.price-up{
    color:green;
    font-weight:bold;
    margin-top:10px;}
.price-down{
    color:red;
    font-weight:bold;
    margin-top:10px;}
.table-box{
    background:#fff;
    border-radius:15px;
    padding:25px;
    border:1px solid var(--border);}
.market-table{
    width:100%;
    border-collapse:collapse;
    margin-top:15px;}
.market-table th,
.market-table td{
    padding:15px;
    border-bottom:1px solid #eee;
    text-align:left;}
.market-table th{
    color:#FF;
    font-size:13px;}
footer{
    background:#CCFFFF;
    border-top:1px solid var(--border);
    padding:40px 5% 20px;
    text-align:center;
    margin-top:40px;}
.quote{
    background:var(--red);
    color:#fff;
    padding:10px 25px;
    border-radius:25px;
    display:inline-block;
    margin-bottom:25px;}
.footer-logo{
    font-size:28px;
    font-weight:bold;
    margin-bottom:20px;}
.social a{
    font-size:20px;
    margin:0 10px;
    color:var(--light);}
.social a:hover{
    color:var(--primary);}
.footer-links{
    margin:25px 0;}
.footer-links a{
    margin:0 10px;
    font-size:14px;
    font-weight:500;
    text-decoration:none;
    color:#000;}
.footer-desc{
    max-width:600px;
    margin:auto;
    font-size:13px;
    color:var(--light);
    line-height:1.6;}
.copyright{
    margin-top:20px;
    font-size:12px;
    color:#bdc3c7;
    border-top:1px solid #eee;
    padding-top:15px;}
  .video-box{
    position:relative;
    padding-bottom:56.25%;
    overflow:hidden;
    border-radius:10px;
}

.video-box iframe{
    position:absolute;
    width:100%;
    height:100%;
}
</style>
</head>
<body>
<header>
<div class="header-top">
    <div class="brand">
        <div class="brand-text">
            <span class="brand-top">A8K60</span>
            <span class="brand-main">TRỊNH HÀ NINH</span>
            <div class="brand-bottom-row">
                <span class="brand-bottom">CMA</span>
                <img src="unnamed.png" class="logo">
            </div>
        </div>
        <span class="date-vertical">HN-12-02-2026</span>
    </div>
    <div class="auth">
        <a href="#">Đăng nhập</a>
        <a href="#">Đăng ký</a>
    </div>
</div>
<div class="banner">
    <div class="banner-content">
        <h1>CHỨNG KHOÁN - CỔ PHIẾU CMA</h1>
        <p>Hãy giữ một cái đầu lạnh để đầu tư thông minh !</p>
    </div>
</div>
<nav>
    <a href="#">Trang chủ</a>
    <a href="https://banggia.vps.com.vn/chung-khoan/HOSE">HOSE</a>
    <a href="https://hnx.vn/vi-vn/trang-chu-mobile.html">HNX</a>
    <a href="https://iboard.ssi.com.vn/">Bảng giá</a>
    <a href="http://c3chuongmya.edu.vn/">Tin tức</a>
    <a href="https://vietstock.vn/chung-khoan.htm">Hỗ trợ</a>
</nav>
</header>
<main>
  <h2 class="section-title">VIDEO HƯỚNG DẪN ĐẦU TƯ</h2>

<div class="video-box">
    <iframe src="https://www.youtube.com/embed/8c1rSMYAbIU" frameborder="0" allowfullscreen></iframe>
</div>
<p class="video-desc">
        Video cung cấp góc nhìn trực quan về cách thị trường vận hành, cách dòng tiền di chuyển 
        và cách một nhà đầu tư phân tích dữ liệu trước khi đưa ra quyết định.
    </p>
<section class="article">
    <h2 class="section-title">GIỚI THIỆU</h2>

    <p>
        Đây là mô hình mô phỏng thị trường chứng khoán trong môi trường học sinh.
        Hệ thống được xây dựng nhằm tái hiện cách giá biến động, cách dòng tiền di chuyển
        và cách nhà đầu tư đưa ra quyết định.
    </p>

    <p>
        Mục tiêu chính không phải kiếm lợi nhuận mà là rèn luyện tư duy phân tích,
        kỷ luật và khả năng kiểm soát rủi ro.
    </p>
</section>

<section class="article">
    <h2 class="section-title">CÁCH THỊ TRƯỜNG HOẠT ĐỘNG</h2>

    <p>
        Giá cổ phiếu thay đổi dựa trên cung và cầu.
        Khi nhiều người mua hơn bán, giá tăng.
        Khi nhiều người bán hơn mua, giá giảm.
    </p>

    <p>
        Tuy nhiên, phía sau đó là tâm lý đám đông và dòng tiền lớn.
        Người tham gia cần quan sát dữ liệu thay vì phản ứng theo cảm xúc.
    </p>
</section>

<section class="article">
    <h2 class="section-title">CHIẾN LƯỢC</h2>

    <p>
        Một chiến lược cơ bản cần tuân thủ các nguyên tắc:
    </p>

    <ul>
        <li>Không dồn vốn vào một mã</li>
        <li>Có điểm cắt lỗ rõ ràng</li>
        <li>Không mua theo tin đồn</li>
        <li>Ưu tiên xu hướng thị trường</li>
    </ul>
</section>

<section class="article">
    <h2 class="section-title">QUẢN LÝ RỦI RO</h2>

    <p>
        Không có phương pháp nào đảm bảo thắng liên tục.
        Điều quan trọng là hạn chế thua lỗ lớn.
    </p>

    <p>
        Giữ được vốn giúp duy trì khả năng tham gia thị trường lâu dài.
    </p>
</section>
<div class="search-bar">
    <i class="fas fa-search"></i>
    <input placeholder="Tìm kiếm mã chứng khoán">
    <i class="fas fa-microphone"></i>
</div>
<section class="hero">
<div class="chart-box">
<svg viewBox="0 0 500 200">
<defs>
<linearGradient id="grad" x1="0%" y1="0%" x2="0%" y2="100%">
<stop offset="0%" stop-color="#2ecc71" stop-opacity="0.3"/>
<stop offset="100%" stop-color="#2ecc71" stop-opacity="0"/>
</linearGradient>
</defs>
<path
d="M0,150 L80,130 L160,140 L240,90 L320,110 L400,50 L480,70 L500,40 L500,200 L0,200 Z"
fill="url(#grad)"/>
<path class="line"
d="M0,150 L80,130 L160,140 L240,90 L320,110 L400,50 L480,70 L500,40"/>
</svg>
</div>
<div class="marquee-text">
<div class="marquee-content">
SÀN CHỨNG KHOÁN TRƯỜNG THPT CMA
</div>
</div>
</section>
<h2 class="section-title">CỔ PHIẾU HOT</h2>
<div class="stock-grid">
<div class="stock-card">
<h3>VCF</h3>
<h5>Lớp 10A10</h5>
<p class="price-down">-0.6% <i class="fas fa-caret-down"></i></p>
</div>
<div class="stock-card">
<h3>VTP</h3>
<h5>Lớp 12A8</h5>
<p class="price-up">+5.2% <i class="fas fa-caret-up"></i></p>
</div>
<div class="stock-card">
<h3>PWG</h3>
<h5>Lớp 11A5</h5>
<p class="price-up">+2.9% <i class="fas fa-caret-up"></i></p>
</div>
<div class="stock-card">
<h3>HGM</h3>
<h5>Lớp 12A1</h5>
<p class="price-down">-1.1% <i class="fas fa-caret-down"></i></p>
</div>
</div>
<div class="table-box">
<h3>Bảng giá trực tuyến</h3>
<table class="market-table">
<thead>
<tr>
<th>MÃ CP</th>
<th>GIÁ</th>
<th>THAY ĐỔI</th>
<th>KHỐI LƯỢNG</th>
<th>XU HƯỚNG</th>
</tr>
</thead>
<tbody>
    <tr>
<td><strong>10A10</strong></td>
<td>10,000</td>
<td class="price-down">-500</td>
<td>86,100</td>
<td><i class="fas fa-chart-line price-down"></i></td>
</tr>
<tr>
<td><strong>12A8</strong></td>
<td>30,300</td>
<td class="price-up">+4,500</td>
<td>195,500</td>
<td><i class="fas fa-chart-line price-up"></i></td>
</tr>
    <tr>
<td><strong>11A5</strong></td>
<td>24,500</td>
<td class="price-up">+1,200</td>
<td>154,200</td>
<td><i class="fas fa-chart-line price-up"></i></td>
</tr>
<td><strong>12A1</strong></td>
<td>11,800</td>
<td class="price-down">-900</td>
<td>100,800</td>
<td><i class="fas fa-chart-line price-down"></i></td>
</tr>
</tbody>
</table>
</div>
</main>
<footer>
<div class="quote">
⭐ Tôi yêu Việt Nam ❤️🇻🇳
</div>
<div class="footer-logo">NINH🤓🤑</div>
<div class="social">
 <a href="#"<i class="fab fa-telegram"></i></a>
        <a href="#"<i class="fab fa-discord"></i></a>
        <a href="#"<i class="fab fa-x-twitter"></i></a>
        <a href="#"<i class="fab fa-facebook"></i></a>
        <a href="#"<i class="fab fa-tiktok"></i></a>
        <a href="#"<i class="fab fa-youtube"></i></a>
        <a href="#"<i class="fab fa-instagram"></i></a>
    </div>
    <div class="footer-links">
        <a href="#">Hỏi đáp</a>
        <a href="#">Chính sách bảo mật</a>
        <a href="#">Điều khoản sử dụng</a>
        <a href="#">Giới thiệu</a>
        <a href="#">Liên hệ</a>
    </div>
<p class="footer-desc">
    <p></p>Website chứng khoán <strong>CMA</strong> do <strong>TRỊNH HÀ NINH</strong> thành lập.</p>Đồng hành và tài trợ chính bởi <strong>GEMINI , CHAT GPT</strong>.
</p>
<div class="copyright">
© 2026 - 12A8K60CMA
              <img src="file:///storage/emulated/0/Download/FB_IMG_17710752708149957-removebg-preview.png" class="logo">       
        </div>
</footer>
</body>
</html>
