<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #d3d3d3; /* 회색 배경 설정 */
        }
        .navbar {
            background-color: #333;
            overflow: hidden;
        }
        .navbar a {
            float: left;
            display: block;
            color: #f2f2f2;
            text-align: center;
            padding: 14px 20px;
            text-decoration: none;
        }
        .navbar a:hover {
            background-color: #ddd;
            color: black;
        }
        .container {
            width: 80%;
            margin: auto;
            overflow: hidden;
            background: #fff;
            padding: 20px;
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }
        .product-images {
            display: flex;
            justify-content: center;
            position: relative; /* relative positioning to contain the absolute positioned text */
        }
        .product-images img {
            max-width: 100%;
            height: auto;
            border: 1px solid #ddd;
            padding: 10px;
        }
        .most-popular-section {
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            margin-top: 20px;
        }
        .most-popular {
            font-weight: bold;
            margin: 0;
        }
        .popular-items {
            display: flex;
            gap: 20px;
            margin-top: 10px;
        }
        .product {
            background: #fff;
            border: 1px solid #ddd;
            border-radius: 10px;
            overflow: hidden;
            text-align: center;
            width: 22%;
        }
        .product img {
            width: 100%;
            height: auto;
        }
        .product p {
            margin: 10px 0;
            font-weight: bold;
        }
        .more-btn-container {
            display: flex;
            justify-content: center;
            margin-top: 20px;
            width: 100%;
        }
        .more-btn {
            background-color: #007bff;
            color: #fff;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }
        .more-btn:hover {
            background-color: #0056b3;
        }
        /* 팝업 스타일 */
        .popup {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5);
            display: none;
            align-items: center;
            justify-content: center;
        }
        .popup-content {
            background-color: #fff;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            max-width: 500px;
            width: 80%;
        }
        .popup-content h2 {
            margin: 0 0 20px;
        }
        .popup-content p {
            margin: 0 0 20px;
        }
        .close-btn {
            background-color: #007bff;
            color: #fff;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
        }
        .close-btn:hover {
            background-color: #0056b3;
        }

        /* 상단 오른쪽 메뉴 스타일 */
        .top-menu {
            display: flex;
            justify-content: flex-end;
            background-color: #333;
            padding: 10px;
        }
        .top-menu a {
            color: #f2f2f2;
            text-decoration: none;
            margin-left: 15px;
            padding: 5px 10px;
            font-size: 12px; /* 글씨 크기를 작게 설정 */
        }
        .top-menu a:hover {
            background-color: #ddd;
            color: black;
        }
    </style>
</head>
<body>

<!-- 상단 오른쪽 메뉴 -->
    <div class="top-menu">
        <a href="https://blog.naver.com/kb781243#customer-service">고객센터</a>
        <a href="https://blog.naver.com/kb781243#my-page">마이페이지</a>
        <a href="https://blog.naver.com/kb781243#wishlist">관심</a>
        <a href="https://blog.naver.com/kb781243#notifications">알림</a>
        <a href="https://blog.naver.com/kb781243#login">로그인</a>
    </div>

    <h1 style="text-align: center;">FM_CROSSFIT SHOP</h1>

    <div class="navbar">
        <a href="https://blog.naver.com/kb781243#best">BEST</a>
        <a href="https://blog.naver.com/kb781243#shoes">SHOES</a>
        <a href="https://blog.naver.com/kb781243#apparel">APPAREL</a>
        <a href="https://blog.naver.com/kb781243#cap">CAP</a>
        <a href="https://blog.naver.com/kb781243#socks">SOCKS</a>
    </div>

<div class="container">
    <div class="product-images">
        <img src="https://assets.roguefitness.com/f_auto,q_auto,c_fill,g_center,w_1200,h_800/homepage/2024%20Q2/mobile-2_uka7jd.jpg" alt="상품 이미지">
    </div>

    <!-- Most Popular Section -->
    <div class="most-popular-section">
        <h2 class="most-popular">Most Popular</h2>
        <p>인기 상품</p>
        <div class="popular-items">
            <div class="product">
                <img src="https://static.nike.com/a/images/t_PDP_1728_v1/f_auto,q_auto:eco/i1-9fe1a65e-c459-4f81-a4f0-8b1b1a188004/%EB%A1%9C%EB%A7%90%EB%A0%88%EC%98%A4-4-%EC%97%AD%EB%8F%84%ED%99%94-jXJbs6Sl.png" alt="Product 1">
                <p style="font-size: 10px;">나이키 로말레오4 역도화</p>
                <p>₩329,000</p>
            </div>
            <div class="product">
                <img src="https://static.nike.com/a/images/t_PDP_1728_v1/f_auto,q_auto:eco/24231b12-64f5-4957-adc6-525518d4ecfb/%EB%A9%94%ED%8A%B8%EC%BD%98-9-%EC%9D%B4%EC%A7%80%EC%98%A8-%EB%82%A8%EC%84%B1-%EC%9A%B4%EB%8F%99%ED%99%94-NipJztjo.png" alt="Product 2">
                <p style="font-size: 10px;">메트콘 9 이지온 남성 운동화</p>
                <p>₩149,000</p>
            </div>
            <div class="product">
                <img src="https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/f8eca38a-d233-44df-b7e5-a3ba62e93c7c/nocta-%EB%82%A8%EC%84%B1-%EB%93%9C%EB%9D%BC%EC%9D%B4-%ED%95%8F-%EC%A0%80%EC%A7%80-ALdTNkTJ.png" alt="Product 3">
                <p style="font-size: 10px;">NOCTA BASKETBALL JERSEY</p>
                <p>₩129,000</p>
            </div>
            <div class="product">
                <img src="https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/8986d7dc-7d79-47c3-af31-ee028b435571/%EC%8A%A4%ED%8F%AC%EC%B8%A0%EC%9B%A8%EC%96%B4-%EB%82%A8%EC%84%B1-%EB%A7%A5%EC%8A%A490-%ED%8B%B0%EC%85%94%EC%B8%A0-U3I3hxUH.png" alt="Product 4">
                <p style="font-size: 10px;">나이키 스포츠웨어 남성 포토 티셔츠</p>
                <p>₩35,000</p>
            </div>
        </div>
    </div>

    </script>
    </script>
    <!DOCTYPE html>
    <html lang="ko">
    <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>더보기 </title>
    <style>
      /* 간단한 스타일링 */
      .more-btn-container {
        text-align: center;
        margin: 20px 0;
      }
      .more-btn {
        padding: 10px 20px;
        font-size: 16px;
        cursor: pointer;
      }
      #more-products {
        display: none; /* 초기에는 숨김 */
        padding: 20px;
        border: 1px solid #ccc;
        margin-top: 20px;
        overflow-x: auto; /* 넘치는 경우 스크롤 표시 */
      }
      #more-products.visible {
        display: block; /* 버튼 클릭 시 보이게 함 */
      }
      #more-products ul {
        list-style-type: none;
        padding: 0;
        margin: 0;
        display: flex; /* 가로로 나열 */
        flex-wrap: nowrap; /* 가로로 넘칠 경우 스크롤 가능하게 설정 */
      }
      #more-products ul li {
        margin-right: 10px;
      }
      #more-products ul li img {
        max-width: 150px; /* 이미지 최대 너비 설정 */
        height: auto; /* 이미지 높이 자동 조정 */
        display: block; /* 인라인 요소를 블록으로 변환하여 여백 조절 */
        margin-bottom: 10px; /* 이미지 아래 여백 추가 */
      }
    </style>
    </head>
    <body>

    <div class="more-btn-container">
      <button class="more-btn" onclick="showMoreProducts()">더보기</button>
    </div>

    <div id="more-products">
      <!-- 추가 상품들이 나타날 공간 -->
    </div>

    <script>
      function showMoreProducts() {
        const moreProductsSection = document.getElementById('more-products');
        if (moreProductsSection) {
          // 추가 상품 섹션을 보이도록 클래스 추가
          moreProductsSection.classList.add('visible');
          // 추가 상품들을 HTML에 추가
          moreProductsSection.innerHTML = `
            <h3>함께 보면 좋은 상품들 </h3>
            <ul>
              <li>
                <img src="https://static.nike.com/a/images/t_PDP_1728_v1/f_auto,q_auto:eco/e63dbd11-199c-44a6-b01a-67c5865f1750/%EC%9D%B8%EB%B9%88%EC%84%9C%EB%B8%94-3-%EB%82%A8%EC%84%B1-%EB%A1%9C%EB%93%9C-%EB%9F%AC%EB%8B%9D%ED%99%94-rvMRfiCS.png" alt="상품 1">
              </li>
              <li>
                <img src="https://static.nike.com/a/images/t_PDP_1728_v1/f_auto,q_auto:eco/7a7d32fe-76ec-4ab6-9d7c-d3a38068917f/%EC%9A%B8%ED%8A%B8%EB%9D%BC%ED%94%8C%EB%9D%BC%EC%9D%B4-%EB%82%A8%EC%84%B1-%ED%8A%B8%EB%A0%88%EC%9D%BC-%EB%A0%88%EC%9D%B4%EC%8B%B1%ED%99%94-imIxlPMv.png" alt="상품 2">
              </li>
              <li>

              <li>
                <img src="https://static.nike.com/a/images/t_PDP_1728_v1/f_auto,q_auto:eco/75bc7c02-f18c-43d3-9456-2d00bb6d5e30/%EC%A0%80%EB%8B%88-%EB%9F%B0-%EB%82%A8%EC%84%B1-%EB%A1%9C%EB%93%9C-%EB%9F%AC%EB%8B%9D%ED%99%94-8HXfWyyi.png" alt="상품 4">
              </li>
            </ul>
          `;
          // 추가 상품 섹션으로 부드럽게 스크롤
          moreProductsSection.scrollIntoView({ behavior: 'smooth', block: 'start' });
        }
      }
    </script>

    </body>
    </html>
    <!-- 팝업 창 -->
    <div class="popup" id="popup">
        <div class="popup-content">
            <h2>이벤트에 오신 것을 환영합니다!</h2>
            <p>오늘 구매하시면 특별 할인을 받을 수 있습니다.</p>
            <button class="close-btn" onclick="goToProduct()">제품보러가기</button>
        </div>
    </div>

    <script>
        // 페이지 로드 시 팝업 표시
        window.onload = function() {
            document.getElementById('popup').style.display = 'flex';
        }

        // 팝업 닫기 및 제품 페이지로 이동 함수
        function goToProduct() {
            document.getElementById('popup').style.display = 'none';
            // 제품 페이지로 이동
            window.location.href = "#shoes"; // 링크를 실제 제품 페이지로 변경
        }
    </script>

    </body>
    </html>