[Uploading index.html…]()
<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cổng Đăng ký & Tra cứu kết quả tuyển sinh | USSH-VNUHCM</title>
<style>
  :root{
    --blue:#0046a8;
    --blue2:#063b8d;
    --red:#c81d25;
    --gold:#f2c94c;
    --text:#263238;
    --muted:#667085;
    --line:#e5e7eb;
    --bg:#f5f7fb;
    --white:#fff;
  }
  *{box-sizing:border-box}
  html{scroll-behavior:smooth}
  body{
    margin:0;
    font-family:Arial,Helvetica,sans-serif;
    color:var(--text);
    background:var(--bg);
  }
  a{text-decoration:none;color:inherit}
  button,input{font:inherit}

  .topbar{
    background:var(--blue2);
    color:#fff;
    font-size:13px;
  }
  .container{max-width:1180px;margin:auto;padding:0 18px}
  .topbar .inner{
    min-height:36px;display:flex;align-items:center;
    justify-content:space-between;gap:18px;
  }
  .top-links{display:flex;gap:20px;flex-wrap:wrap}
  .top-links a:hover{color:#dbeafe}

  header{
    background:#fff;
    border-bottom:1px solid #dce2ea;
    position:sticky;top:0;z-index:20;
  }
  .head{
    min-height:92px;display:flex;align-items:center;
    justify-content:space-between;gap:25px;
  }
  .brand{display:flex;align-items:center;gap:14px}
  .logo{
    width:58px;height:58px;border-radius:50%;
    border:3px solid var(--blue);
    display:grid;place-items:center;
    color:var(--blue);font-weight:800;font-size:20px;
    background:#fff;
  }
  .brand-title{
    color:var(--blue2);font-weight:800;font-size:20px;
    line-height:1.25;text-transform:uppercase;
  }
  .brand-sub{font-size:12px;color:#6b7280;margin-top:4px}
  nav{display:flex;align-items:center;gap:4px;flex-wrap:wrap}
  nav a{
    padding:12px 11px;border-radius:5px;font-size:14px;
    color:#263b62;font-weight:600;
  }
  nav a:hover,nav a.active{background:#edf4ff;color:var(--blue)}

  .hero{
    background:linear-gradient(120deg,#003d91,#075bc7);
    color:#fff;
    position:relative;overflow:hidden;
  }
  .hero:after{
    content:"";position:absolute;width:380px;height:380px;
    border-radius:50%;right:-120px;top:-170px;
    background:rgba(255,255,255,.08);
  }
  .hero .inner{
    min-height:280px;display:grid;grid-template-columns:1.25fr .75fr;
    gap:30px;align-items:center;position:relative;z-index:1;
  }
  .eyebrow{font-size:14px;letter-spacing:.5px;opacity:.9;margin-bottom:10px}
  h1{font-size:34px;line-height:1.2;margin:0 0 12px}
  .hero p{max-width:690px;line-height:1.7;margin:0 0 22px;color:#eaf2ff}
  .hero-actions{display:flex;gap:10px;flex-wrap:wrap}
  .btn{
    border:0;border-radius:6px;padding:12px 18px;
    cursor:pointer;font-weight:700;transition:.2s;
  }
  .btn-primary{background:#fff;color:var(--blue)}
  .btn-primary:hover{transform:translateY(-1px)}
  .btn-outline{background:transparent;color:#fff;border:1px solid rgba(255,255,255,.65)}
  .btn-blue{background:var(--blue);color:#fff}
  .btn-blue:hover{background:#00377f}
  .hero-card{
    background:rgba(255,255,255,.11);
    border:1px solid rgba(255,255,255,.2);
    border-radius:12px;padding:22px;
    backdrop-filter:blur(5px);
  }
  .hero-card h3{margin:0 0 15px;font-size:18px}
  .hero-card .item{
    display:flex;justify-content:space-between;gap:20px;
    padding:10px 0;border-bottom:1px solid rgba(255,255,255,.17);
    font-size:14px;
  }
  .hero-card .item:last-child{border-bottom:0}

  main{padding:35px 0 45px}
  .section-title{text-align:center;margin-bottom:24px}
  .section-title h2{color:var(--blue2);margin:0 0 7px;font-size:25px}
  .section-title p{margin:0;color:var(--muted);font-size:14px}

  .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
  .card{
    background:#fff;border:1px solid var(--line);border-radius:10px;
    padding:23px;box-shadow:0 3px 12px rgba(15,23,42,.045);
  }
  .card-icon{
    width:44px;height:44px;border-radius:8px;background:#eaf2ff;
    color:var(--blue);display:grid;place-items:center;
    font-size:21px;font-weight:800;margin-bottom:14px;
  }
  .card h3{font-size:17px;color:#153d7a;margin:0 0 8px}
  .card p{font-size:14px;color:#667085;line-height:1.6;margin:0 0 15px}
  .card a{color:var(--blue);font-size:14px;font-weight:700}

  .info{
    margin-top:30px;background:#fff;border:1px solid var(--line);
    border-radius:10px;padding:25px;
  }
  .info h2{font-size:20px;color:var(--blue2);margin:0 0 16px}
  .notice{
    border-left:4px solid var(--red);background:#fff8f8;
    padding:13px 15px;margin-bottom:18px;line-height:1.6;font-size:14px;
  }
  .news{display:grid;grid-template-columns:repeat(2,1fr);gap:12px}
  .news-item{
    padding:14px;border:1px solid var(--line);border-radius:8px;
    transition:.2s;background:#fff;
  }
  .news-item:hover{border-color:#b9d0f4;transform:translateY(-1px)}
  .date{font-size:12px;color:var(--red);font-weight:700;margin-bottom:6px}
  .news-item strong{font-size:14px;line-height:1.45;display:block}

  footer{
    background:#062f72;color:#dce8ff;
    margin-top:0;
  }
  .footer-main{
    padding:30px 0;display:grid;grid-template-columns:1.3fr .8fr .8fr;gap:30px;
  }
  footer h3{color:#fff;font-size:16px;margin:0 0 12px}
  footer p,footer li{font-size:13px;line-height:1.7;color:#c6d5ee}
  footer ul{padding:0;margin:0;list-style:none}
  footer li{margin:4px 0}
  .simulation-note{
    text-align:center;border-top:1px solid rgba(255,255,255,.13);
    padding:12px 18px;font-size:11px;color:#aebfdc;
    letter-spacing:.15px;
  }



  .lookup-page{
    display:none;
    min-height:calc(100vh - 36px);
    background:linear-gradient(145deg,#063b8d 0%,#075bc7 48%,#eef4fb 100%);
    position:relative;overflow:hidden;
    padding-bottom:35px;
  }
  .lookup-page.show{display:block}
  .lookup-page:before,.lookup-page:after{
    content:"";position:absolute;border:1px solid rgba(255,255,255,.12);
    border-radius:50%;pointer-events:none;
  }
  .lookup-page:before{width:480px;height:480px;right:-190px;top:65px}
  .lookup-page:after{width:650px;height:650px;right:-310px;top:-20px}
  .lookup-header{
    height:55px;background:#0750a8;color:#fff;display:flex;
    align-items:center;justify-content:space-between;padding:0 14px;
    position:relative;z-index:2;box-shadow:0 1px 4px rgba(0,0,0,.15);
  }
  .lookup-brand{display:flex;align-items:center;gap:8px}
  .lookup-brand-logo{
    width:24px;height:24px;border-radius:50%;background:#fff;
    color:#0750a8;display:grid;place-items:center;font-size:7px;font-weight:900;
  }
  .lookup-brand-title{font-size:8px;font-weight:900;line-height:1.15}
  .lookup-brand-sub{font-size:6px;margin-top:2px;opacity:.9}
  .lookup-menu{font-size:22px;line-height:1}
  .lookup-title{
    max-width:390px;margin:0 auto;padding:25px 15px 62px;
    color:#fff;position:relative;z-index:1;
  }
  .lookup-title h1{
    font-size:21px;margin:0;font-weight:900;line-height:1.25;
  }
  .lookup-title p{font-size:9px;margin:6px 0 0;color:#dceaff}
  .lookup-panel{
    width:min(390px,calc(100% - 18px));margin:-28px auto 0;
    background:#fff;border-radius:11px;padding:13px 11px 12px;
    position:relative;z-index:3;box-shadow:0 7px 22px rgba(0,45,100,.16);
  }
  .lookup-panel-head{display:flex;align-items:center;gap:8px;margin-bottom:12px}
  .search-icon{
    width:25px;height:25px;border-radius:7px;background:#e8eff9;
    color:#1456a6;display:grid;place-items:center;font-size:13px;font-weight:900;
  }
  .lookup-panel-head strong{font-size:12px;color:#344054}
  .lookup-step{margin-bottom:9px}
  .step-label{
    display:flex;align-items:center;gap:5px;margin-bottom:5px;
    font-size:8px;font-weight:800;color:#475467;
  }
  .step-no{
    width:15px;height:15px;border-radius:50%;background:#eaf1fa;
    color:#1756a0;display:grid;place-items:center;font-size:8px;
  }
  .lookup-input,.lookup-select{
    width:100%;height:35px;border:1px solid #d9e0e9;border-radius:8px;
    background:#fff;padding:0 10px;font-size:10px;color:#344054;outline:none;
  }
  .lookup-input:focus,.lookup-select:focus{
    border-color:#1762bb;box-shadow:0 0 0 3px #e9f2ff;
  }
  .lookup-select{appearance:auto}
  .lookup-submit{
    width:100%;height:36px;border:0;border-radius:8px;
    background:linear-gradient(90deg,#06439a,#0868c8);
    color:#fff;font-size:10px;cursor:pointer;font-weight:700;
    box-shadow:0 3px 8px rgba(5,73,158,.25);
    margin-top:2px;
  }
  .lookup-note{text-align:center;color:#98a2b3;font-size:7px;margin-top:8px}
  .lookup-error{display:none;color:#b42318;font-size:8px;margin:5px 0 0}

  .result-page{
    display:none;
    min-height:calc(100vh - 128px);
    background:#f1f4f8;
    padding-bottom:30px;
  }
  .result-page.show{display:block}
  .result-top{
    height:52px;background:#fff;border-bottom:1px solid #d9dee7;
    display:flex;align-items:center;justify-content:space-between;
    padding:0 18px;font-size:13px;color:#475467;
  }
  .result-top .back{cursor:pointer;font-weight:600;color:#475467}
  .result-top .brand-mini{font-weight:800;color:#123b7a}
  .result-wrap{max-width:390px;margin:0 auto;padding:12px 10px 0}
  .result-card{
    position:relative;overflow:hidden;
    border-radius:13px;
    padding:15px 14px 20px;
    color:#fff;
    background:linear-gradient(150deg,#06346f 0%,#0755a9 54%,#1267c2 100%);
    box-shadow:0 4px 12px rgba(15,48,92,.22);
    border:1px solid rgba(255,255,255,.25);
  }
  .result-card:after{
    content:"USSH";position:absolute;right:10px;bottom:-10px;
    font-size:66px;font-weight:900;letter-spacing:-5px;
    color:rgba(255,255,255,.055);pointer-events:none;
  }
  .result-head{
    display:flex;align-items:center;justify-content:space-between;
    position:relative;z-index:1;margin-bottom:26px;
  }
  .school{display:flex;align-items:center;gap:9px}
  .school-logo{
    width:27px;height:27px;border-radius:50%;background:#fff;
    display:grid;place-items:center;color:#0755a9;font-size:9px;font-weight:900;
    border:1px solid #dce8fa;
  }
  .school-name{font-size:11px;font-weight:800;line-height:1.2}
  .school-sub{font-size:7px;opacity:.88;margin-top:2px}
  .national-badge{
    border:1px solid rgba(255,255,255,.45);border-radius:12px;
    padding:5px 8px;font-size:8px;font-weight:700;
  }
  .congrats{
    position:relative;z-index:1;font-size:9px;color:#d5e4fa;margin-bottom:3px;
  }
  .candidate-name{
    position:relative;z-index:1;font-size:23px;font-weight:900;
    letter-spacing:-.3px;margin-bottom:10px;
  }
  .admitted{
    position:relative;z-index:1;font-size:8px;color:#d7e5f8;
  }
  .major{
    position:relative;z-index:1;color:#ffd75a;font-size:16px;font-weight:900;
    margin-top:4px;margin-bottom:14px;
  }
  .result-grid{
    position:relative;z-index:1;display:grid;grid-template-columns:1fr 1fr;
    gap:8px;margin-bottom:8px;
  }
  .result-box{
    background:rgba(255,255,255,.075);
    border:1px solid rgba(255,255,255,.12);
    border-radius:8px;padding:9px 10px;min-height:51px;
  }
  .result-box .label{
    display:flex;align-items:center;gap:5px;
    color:#b9d0ec;font-size:7px;text-transform:uppercase;
    font-weight:700;margin-bottom:4px;
  }
  .result-box .value{font-size:10px;font-weight:800;color:#fff}
  .result-box .value.large{font-size:11px}
  .result-section{
    position:relative;z-index:1;
    background:rgba(255,255,255,.075);
    border:1px solid rgba(255,255,255,.12);
    border-radius:8px;padding:9px 10px;margin-top:8px;
  }
  .result-row{
    display:flex;justify-content:space-between;gap:15px;
    padding:7px 0;border-bottom:1px solid rgba(255,255,255,.09);
    font-size:8px;
  }
  .result-row:last-child{border-bottom:0}
  .result-row .k{color:#b9d0ec;text-transform:uppercase}
  .result-row .v{font-weight:800;text-align:right}
  .result-footer{
    position:relative;z-index:1;margin-top:12px;
    font-size:7px;color:#c5d9ef;line-height:1.5
  }
  .result-actions{
    max-width:390px;margin:12px auto 0;padding:0 10px;
    display:flex;gap:8px;
  }
  .result-actions button{flex:1}
  @media(max-width:600px){
  
  .lookup-page{
    display:none;
    min-height:calc(100vh - 36px);
    background:linear-gradient(145deg,#063b8d 0%,#075bc7 48%,#eef4fb 100%);
    position:relative;overflow:hidden;
    padding-bottom:35px;
  }
  .lookup-page.show{display:block}
  .lookup-page:before,.lookup-page:after{
    content:"";position:absolute;border:1px solid rgba(255,255,255,.12);
    border-radius:50%;pointer-events:none;
  }
  .lookup-page:before{width:480px;height:480px;right:-190px;top:65px}
  .lookup-page:after{width:650px;height:650px;right:-310px;top:-20px}
  .lookup-header{
    height:55px;background:#0750a8;color:#fff;display:flex;
    align-items:center;justify-content:space-between;padding:0 14px;
    position:relative;z-index:2;box-shadow:0 1px 4px rgba(0,0,0,.15);
  }
  .lookup-brand{display:flex;align-items:center;gap:8px}
  .lookup-brand-logo{
    width:24px;height:24px;border-radius:50%;background:#fff;
    color:#0750a8;display:grid;place-items:center;font-size:7px;font-weight:900;
  }
  .lookup-brand-title{font-size:8px;font-weight:900;line-height:1.15}
  .lookup-brand-sub{font-size:6px;margin-top:2px;opacity:.9}
  .lookup-menu{font-size:22px;line-height:1}
  .lookup-title{
    max-width:390px;margin:0 auto;padding:25px 15px 62px;
    color:#fff;position:relative;z-index:1;
  }
  .lookup-title h1{
    font-size:21px;margin:0;font-weight:900;line-height:1.25;
  }
  .lookup-title p{font-size:9px;margin:6px 0 0;color:#dceaff}
  .lookup-panel{
    width:min(390px,calc(100% - 18px));margin:-28px auto 0;
    background:#fff;border-radius:11px;padding:13px 11px 12px;
    position:relative;z-index:3;box-shadow:0 7px 22px rgba(0,45,100,.16);
  }
  .lookup-panel-head{display:flex;align-items:center;gap:8px;margin-bottom:12px}
  .search-icon{
    width:25px;height:25px;border-radius:7px;background:#e8eff9;
    color:#1456a6;display:grid;place-items:center;font-size:13px;font-weight:900;
  }
  .lookup-panel-head strong{font-size:12px;color:#344054}
  .lookup-step{margin-bottom:9px}
  .step-label{
    display:flex;align-items:center;gap:5px;margin-bottom:5px;
    font-size:8px;font-weight:800;color:#475467;
  }
  .step-no{
    width:15px;height:15px;border-radius:50%;background:#eaf1fa;
    color:#1756a0;display:grid;place-items:center;font-size:8px;
  }
  .lookup-input,.lookup-select{
    width:100%;height:35px;border:1px solid #d9e0e9;border-radius:8px;
    background:#fff;padding:0 10px;font-size:10px;color:#344054;outline:none;
  }
  .lookup-input:focus,.lookup-select:focus{
    border-color:#1762bb;box-shadow:0 0 0 3px #e9f2ff;
  }
  .lookup-select{appearance:auto}
  .lookup-submit{
    width:100%;height:36px;border:0;border-radius:8px;
    background:linear-gradient(90deg,#06439a,#0868c8);
    color:#fff;font-size:10px;cursor:pointer;font-weight:700;
    box-shadow:0 3px 8px rgba(5,73,158,.25);
    margin-top:2px;
  }
  .lookup-note{text-align:center;color:#98a2b3;font-size:7px;margin-top:8px}
  .lookup-error{display:none;color:#b42318;font-size:8px;margin:5px 0 0}

  .result-page{min-height:calc(100vh - 110px)}
    .result-wrap{max-width:390px}
  }

  .modal{
    position:fixed;inset:0;background:rgba(15,23,42,.55);
    display:none;align-items:center;justify-content:center;
    z-index:100;padding:18px;
  }
  .modal.show{display:flex}
  .modal-box{
    width:min(440px,100%);background:#fff;border-radius:12px;
    box-shadow:0 20px 60px rgba(0,0,0,.25);overflow:hidden;
  }
  .modal-head{
    background:var(--blue);color:#fff;padding:17px 20px;
    display:flex;align-items:center;justify-content:space-between;
  }
  .modal-head h3{margin:0;font-size:18px}
  .close{border:0;background:transparent;color:#fff;font-size:24px;cursor:pointer}
  .modal-body{padding:22px}
  label{display:block;font-size:13px;font-weight:700;color:#344054;margin:0 0 7px}
  input{
    width:100%;padding:11px 12px;border:1px solid #d0d5dd;
    border-radius:6px;outline:none;margin-bottom:15px;
  }
  input:focus{border-color:#6b9fe8;box-shadow:0 0 0 3px #eaf2ff}
  .modal-foot{display:flex;justify-content:flex-end;gap:10px;margin-top:4px}
  .small-note{font-size:12px;color:#667085;line-height:1.5;margin-top:12px}

  @media(max-width:900px){
    .hero .inner{grid-template-columns:1fr;padding-top:45px;padding-bottom:45px}
    .hero-card{display:none}
    nav{display:none}
    .grid{grid-template-columns:1fr}
    .footer-main{grid-template-columns:1fr}
  }
  @media(max-width:600px){
    h1{font-size:27px}
    .head{min-height:75px}
    .brand-title{font-size:15px}
    .logo{width:48px;height:48px;font-size:17px}
    .topbar .inner{justify-content:center}
    .top-links{display:none}
    .news{grid-template-columns:1fr}
  }
</style>
</head>
<body>

<div class="topbar">
  <div class="container inner">
    <div>ĐẠI HỌC QUỐC GIA THÀNH PHỐ HỒ CHÍ MINH</div>
    <div class="top-links">
      <a href="#home">Trang chủ</a>
      <a href="#news">Thông báo</a>
      <a href="#contact">Liên hệ</a>
    </div>
  </div>
</div>

<header>
  <div class="container head">
    <a class="brand" href="#home">
      <div class="logo">USSH</div>
      <div>
        <div class="brand-title">Trường Đại học Khoa học Xã hội và Nhân văn</div>
        <div class="brand-sub">Đại học Quốc gia Thành phố Hồ Chí Minh</div>
      </div>
    </a>
    <nav>
      <a class="active" href="#home">TRANG CHỦ</a>
      <a href="#services">TUYỂN SINH</a>
      <a href="#news">THÔNG BÁO</a>
      <a href="#contact">LIÊN HỆ</a>
    </nav>
  </div>
</header>

<section class="hero" id="home">
  <div class="container inner">
    <div>
      <div class="eyebrow">CỔNG THÔNG TIN TUYỂN SINH ĐẠI HỌC</div>
      <h1>Cổng Đăng ký &amp; Tra cứu kết quả tuyển sinh</h1>
      <p>
        Hệ thống hỗ trợ thí sinh đăng ký tuyển sinh, quản lý hồ sơ
        và tra cứu thông tin kết quả tuyển sinh chính thức.
      </p>
      <div class="hero-actions">
        <button class="btn btn-primary" onclick="openLogin('register')">Đăng ký tuyển sinh</button>
        <button class="btn btn-outline" onclick="showResult()">Tra cứu kết quả</button>
      </div>
    </div>
    <div class="hero-card">
      <h3>Thông tin hỗ trợ</h3>
      <div class="item"><span>Hotline</span><strong>1900 3033</strong></div>
      <div class="item"><span>Điện thoại</span><strong>028 3829 3828</strong></div>
      <div class="item"><span>Nhánh</span><strong>200</strong></div>
      <div class="item"><span>Email</span><strong>tuyensinhdaihoc@hcmussh.edu.vn</strong></div>
    </div>
  </div>
</section>

<main>
  <div class="container" id="services">
    <div class="section-title">
      <h2>Dịch vụ tuyển sinh trực tuyến</h2>
      <p>Lựa chọn chức năng bạn cần thực hiện</p>
    </div>

    <div class="grid">
      <div class="card">
        <div class="card-icon">01</div>
        <h3>Đăng ký tuyển sinh</h3>
        <p>Đăng nhập hệ thống để tạo, cập nhật và quản lý hồ sơ đăng ký tuyển sinh.</p>
        <a href="#" onclick="openLogin('register');return false;">Đăng nhập hệ thống →</a>
      </div>

      <div class="card">
        <div class="card-icon">02</div>
        <h3>Tra cứu kết quả</h3>
        <p>Tra cứu kết quả tuyển sinh chính thức theo thông tin thí sinh đã đăng ký.</p>
        <a href="#" onclick="showResult();return false;">Tra cứu ngay →</a>
      </div>

      <div class="card">
        <div class="card-icon">03</div>
        <h3>Hướng dẫn tuyển sinh</h3>
        <p>Xem các bước đăng ký, cập nhật hồ sơ và những lưu ý quan trọng dành cho thí sinh.</p>
        <a href="#guide">Xem hướng dẫn →</a>
      </div>
    </div>

    <section class="info" id="guide">
      <h2>Thông tin cần biết</h2>
      <div class="notice">
        <strong>Lưu ý:</strong> Thí sinh cần kiểm tra chính xác thông tin cá nhân
        trước khi hoàn tất hồ sơ và thường xuyên theo dõi các thông báo tuyển sinh.
      </div>
      <div class="news" id="news">
        <div class="news-item">
          <div class="date">THÔNG BÁO TUYỂN SINH</div>
          <strong>Thông tin tuyển sinh đại học chính quy và các mốc thời gian quan trọng.</strong>
        </div>
        <div class="news-item">
          <div class="date">HƯỚNG DẪN</div>
          <strong>Hướng dẫn đăng ký, cập nhật hồ sơ và tra cứu thông tin trên hệ thống.</strong>
        </div>
        <div class="news-item">
          <div class="date">LƯU Ý</div>
          <strong>Thí sinh sử dụng đúng email và thông tin đã đăng ký để đăng nhập hệ thống.</strong>
        </div>
        <div class="news-item">
          <div class="date">HỖ TRỢ</div>
          <strong>Liên hệ bộ phận tuyển sinh khi cần hỗ trợ về tài khoản hoặc hồ sơ.</strong>
        </div>
      </div>
    </section>
  </div>
</main>



<section class="lookup-page" id="lookupPage">
  <div class="lookup-header">
    <div class="lookup-brand">
      <div class="lookup-menu">☰</div>
      <div class="lookup-brand-logo">USSH</div>
      <div>
        <div class="lookup-brand-title">CỔNG ĐĂNG KÝ<br>&amp; TRA CỨU KẾT QUẢ TUYỂN SINH</div>
      </div>
    </div>
    <div style="font-size:17px">♟</div>
  </div>

  <div class="lookup-title">
    <h1>Tra cứu kết quả trúng tuyển</h1>
    <p>Nhập thông tin để tra cứu kết quả tuyển sinh</p>
  </div>

  <div class="lookup-panel">
    <div class="lookup-panel-head">
      <div class="search-icon">⌕</div>
      <strong>Tra cứu chính thức</strong>
    </div>

    <div class="lookup-step">
      <div class="step-label"><span class="step-no">1</span> Loại hình tuyển sinh</div>
      <select class="lookup-select" id="admissionType">
        <option value="">Chọn loại hình</option>
        <option>Đại học chính quy</option>
        <option>Phương thức xét tuyển</option>
        <option>Chương trình đào tạo khác</option>
      </select>
    </div>

    <div class="lookup-step">
      <div class="step-label"><span class="step-no">2</span> Đợt tra cứu</div>
      <select class="lookup-select" id="lookupRound">
        <option value="">Chọn đợt tra cứu</option>
        <option>Đợt 1</option>
        <option>Đợt 2</option>
        <option>Đợt bổ sung</option>
      </select>
    </div>

    <div class="lookup-step">
      <div class="step-label"><span class="step-no">3</span> CCCD</div>
      <input class="lookup-input" id="lookupCccd" type="text"
             placeholder="Nhập số CCCD" autocomplete="off">
    </div>

    <div class="lookup-error" id="lookupError">Vui lòng nhập thông tin tra cứu.</div>

    <button class="lookup-submit" onclick="submitLookup()">Xem kết quả &nbsp;➜</button>
    <div class="lookup-note">Bản mô phỏng — dữ liệu nhập vào chỉ dùng để minh họa.</div>
  </div>
</section>

<section class="result-page" id="resultPage">
  <div class="result-top">
    <div class="back" onclick="backToLookup()">← &nbsp;Tra cứu</div>
    <div class="brand-mini">🔴 USSH</div>
  </div>

  <div class="result-wrap">
    <div class="result-card">
      <div class="result-head">
        <div class="school">
          <div class="school-logo">USSH</div>
          <div>
            <div class="school-name">USSH – VNUHCM</div>
            <div class="school-sub">Trường ĐH KHXH&NV, ĐHQG-HCM</div>
          </div>
        </div>
        <div class="national-badge">✓ Trúng tuyển</div>
      </div>

      <div class="congrats">Chúc mừng thí sinh</div>
      <div class="candidate-name">HUỲNH THỊ TRÚC LINH</div>
      <div class="admitted">đã chính thức trúng tuyển ngành:</div>
      <div class="major">Ngôn ngữ Trung Quốc</div>

      <div class="result-grid">
        <div class="result-box">
          <div class="label">▣ &nbsp; CCCD</div>
          <div class="value">079305017321</div>
        </div>
        <div class="result-box">
          <div class="label">▣ &nbsp; Ngày sinh</div>
          <div class="value">18/10/2005</div>
        </div>
        <div class="result-box">
          <div class="label">Khu vực ưu tiên</div>
          <div class="value large">2</div>
        </div>
        <div class="result-box">
          <div class="label">Đối tượng ưu tiên</div>
          <div class="value large">—</div>
        </div>
      </div>

      <div class="result-section">
        <div class="result-row">
          <span class="k">Mã ngành</span>
          <span class="v">7320104</span>
        </div>
        <div class="result-row">
          <span class="k">Chương trình</span>
          <span class="v">Chuẩn</span>
        </div>
        <div class="result-row">
          <span class="k">Hình thức đào tạo</span>
          <span class="v">Chính quy</span>
        </div>
      </div>

      <div class="result-footer">
        BẢN MÔ PHỎNG
      </div>
    </div>

    <div class="result-actions">
      <button class="btn btn-blue" onclick="window.print()">In kết quả</button>
      <button class="btn" onclick="hideResult()">Tra cứu lại</button>
    </div>
  </div>
</section>

<footer id="contact">
  <div class="container footer-main">
    <div>
      <h3>TRƯỜNG ĐẠI HỌC KHOA HỌC XÃ HỘI VÀ NHÂN VĂN</h3>
      <p>Đại học Quốc gia Thành phố Hồ Chí Minh</p>
      <p>10-12 Đinh Tiên Hoàng, Phường Bến Nghé, Thành phố Hồ Chí Minh</p>
    </div>
    <div>
      <h3>THÔNG TIN LIÊN HỆ</h3>
      <ul>
        <li>Hotline: 1900 3033</li>
        <li>Điện thoại: 028 3829 3828</li>
        <li>Nhánh: 200</li>
        <li>Email: tuyensinhdaihoc@hcmussh.edu.vn</li>
      </ul>
    </div>
    <div>
      <h3>LIÊN KẾT</h3>
      <ul>
        <li><a href="#home">Trang chủ</a></li>
        <li><a href="#services">Dịch vụ tuyển sinh</a></li>
        <li><a href="#news">Thông báo</a></li>
        <li><a href="#contact">Liên hệ</a></li>
      </ul>
    </div>
  </div>

  <!-- Dòng ghi chú về bản mô phỏng được đặt ở dưới cùng theo yêu cầu -->
  <div class="simulation-note">
    BẢN MÔ PHỎNG THU NHỎ — giao diện tham khảo, không phải cổng tuyển sinh chính thức.
  </div>
</footer>

<div class="modal" id="loginModal" onclick="closeOnBackdrop(event)">
  <div class="modal-box">
    <div class="modal-head">
      <h3 id="modalTitle">Đăng nhập</h3>
      <button class="close" onclick="closeLogin()" aria-label="Đóng">&times;</button>
    </div>
    <div class="modal-body">
      <label for="email">Email</label>
      <input id="email" type="email" placeholder="Nhập email">

      <label for="password">Mật khẩu</label>
      <input id="password" type="password" placeholder="Nhập mật khẩu">

      <div class="modal-foot">
        <button class="btn" onclick="closeLogin()">Đóng</button>
        <button class="btn btn-blue" onclick="demoLogin()">Đăng nhập</button>
      </div>
      <div class="small-note" id="modalNote">
        Đây là giao diện minh họa; nút đăng nhập không gửi dữ liệu đến hệ thống thật.
      </div>
    </div>
  </div>
</div>

<script>

  function showResult(){
    document.getElementById('lookupPage').classList.add('show');
    document.getElementById('resultPage').classList.remove('show');
    document.querySelector('header').style.display = 'none';
    document.querySelector('.hero').style.display = 'none';
    document.querySelector('main').style.display = 'none';
    document.querySelector('footer').style.display = 'none';
    window.scrollTo({top:0,behavior:'instant'});
  }

  function submitLookup(){
    // Bản mô phỏng: chỉ cần bấm "Xem kết quả", nhập gì cũng có thể xem kết quả.
    document.getElementById('lookupPage').classList.remove('show');
    document.getElementById('resultPage').classList.add('show');
    window.scrollTo({top:0,behavior:'instant'});
  }

  function hideResult(){
    document.getElementById('resultPage').classList.remove('show');
    document.getElementById('lookupPage').classList.remove('show');
    document.querySelector('header').style.display = '';
    document.querySelector('.hero').style.display = '';
    document.querySelector('main').style.display = '';
    document.querySelector('footer').style.display = '';
    window.scrollTo({top:0,behavior:'instant'});
  }

  function backToLookup(){
    document.getElementById('resultPage').classList.remove('show');
    document.getElementById('lookupPage').classList.add('show');
    window.scrollTo({top:0,behavior:'instant'});
  }

  const modal = document.getElementById('loginModal');
  const title = document.getElementById('modalTitle');
  const note = document.getElementById('modalNote');

  function openLogin(type){
    modal.classList.add('show');
    if(type === 'lookup'){
      title.textContent = 'Đăng nhập để tra cứu kết quả tuyển sinh';
      note.textContent = 'Nhập tài khoản của bạn để thực hiện tra cứu kết quả.';
    }else{
      title.textContent = 'Đăng nhập';
      note.textContent = 'Nhập email và mật khẩu để tiếp tục đăng ký tuyển sinh.';
    }
    document.getElementById('email').focus();
  }

  function closeLogin(){
    modal.classList.remove('show');
  }

  function closeOnBackdrop(e){
    if(e.target === modal) closeLogin();
  }

  function demoLogin(){
    alert('Đây là bản giao diện mô phỏng. Chức năng đăng nhập chưa kết nối máy chủ.');
  }

  document.addEventListener('keydown', e => {
    if(e.key === 'Escape') closeLogin();
  });
</script>
</body>
</html>
