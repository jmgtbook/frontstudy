<script>
//    import Home from "./routes/Home";
//    import Jangpocket from "./routes/Jangpocket";
//    import Login from "./routes/login";
//    import Mypage from "./routes/Mypage";
//    import Search from "./routes/Search";
//    import Signup from "./routes/Signup";
//    import Support from "./routes/Support";
//    import Totalsearch from "./routes/Totalsearch";

//    function moveToPage(pageName) {
//     navigate(`/${pageName}`);
//   }
    import {link} from 'svelte-spa-router'

</script>

<header>
    <div class="header">
        <div class="header-2">
          <div class="frame-header-2">
            <div class="frame-19"></div>
          </div>
          <a href="/home" class="chek">CHEK</a>
          <article class="line-7"></article>
          <button on:click={() => link('/Checkchek')} class="button-checkchek">
            <svg
              class="frame-20"
              width="30"
              height="36"
              viewBox="0 0 30 36"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M13.8645 24.3536L2.5 32.1912V2H27.5V32.1912L16.1355 24.3536L15 23.5705L13.8645 24.3536Z"
                fill="#F3F3F3"
                stroke="black"
                stroke-width="4"
              />
            </svg>
          </button>
          <button on:click={() => push('/Totalsearch')} class="button-totalsearch">
            <div class="div">통합검색</div>
            <svg
              class="totalsearchimg"
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M7.28577 9.29289C7.67591 8.90237 8.30845 8.90237 8.6986 9.29289L11.9883 12.5858L15.2779 9.29289C15.6681 8.90237 16.3006 8.90237 16.6907 9.29289C17.0809 9.68342 17.0809 10.3166 16.6907 10.7071L12.6947 14.7071C12.3045 15.0976 11.672 15.0976 11.2818 14.7071L7.28577 10.7071C6.89563 10.3166 6.89563 9.68342 7.28577 9.29289Z"
                fill="black"
              />
            </svg>
          </button>
          <button on:click={() => push('/Search')} class="button-search">
            <svg
              class="icon-search"
              width="36"
              height="36"
              viewBox="0 0 36 36"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <g clip-path="url(#clip0_10_83)">
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M14.6642 0C6.56537 0 0 6.49302 0 14.5026C0 22.5121 6.56537 29.0051 14.6642 29.0051C17.958 29.0051 20.9982 27.9311 23.4462 26.1179L32.2961 35.3932C33.1142 36.2023 34.533 36.2023 35.3511 35.3932C36.1692 34.5841 36.1692 33.1809 35.3511 32.3718L26.4089 23.1879C28.2423 20.7668 29.3283 17.7601 29.3283 14.5026C29.3283 6.49302 22.7629 0 14.6642 0ZM4.18976 14.5026C4.18976 8.78147 8.87931 4.14359 14.6642 4.14359C20.449 4.14359 25.1386 8.78147 25.1386 14.5026C25.1386 20.2237 20.449 24.8616 14.6642 24.8616C8.87931 24.8616 4.18976 20.2237 4.18976 14.5026Z"
                  fill="black"
                />
              </g>
              <defs>
                <clipPath id="clip0_10_83">
                  <rect width="35.9647" height="36" fill="white" />
                </clipPath>
              </defs>
            </svg>
          </button>
          <button on:click={() => push('/Mypage')} class="button-mypage">
            <svg
              class="icon-mypage"
              width="36"
              height="36"
              viewBox="0 0 36 36"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M30.6 33H30.57M30.57 33H5.4C4.08 33 3 31.92 3 30.6V25.125C3 24.75 3 24.555 3.18 24.195C3.75 22.875 5.43 21.765 8.055 20.82M30.57 33C31.89 33 32.97 31.92 32.97 30.6V25.125C32.97 24.765 32.97 24.375 32.79 24.195C32.235 22.89 30.54 21.75 27.915 20.82M18 20.25C13.875 20.25 10.5 16.875 10.5 12.75V10.5C10.5 6.375 13.875 3 18 3C22.125 3 25.5 6.375 25.5 10.5V12.75C25.5 16.875 22.125 20.25 18 20.25Z"
                stroke="black"
                stroke-width="4"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </button>
          <div class="input-search"></div>
        </div>
        <div class="header-1">
          <header class="frame-header-1"></header>
          <div class="frame-18">
            <a href="/login" class="div2">로그인</a>
            <a href="/signup" class="div2">회원가입</a>
            <a href="/jangpocket" class="div2">장바구니</a>
            <a href="/mypage" class="div2">마이페이지</a>
            <a href="/support" class="div2">문의하기</a>
          </div>
        </div>
      </div>
      
      
</header>

<slot/>

<footer>

</footer>

<style>
button{
    background: rgba(255, 255, 255, 0);
    border:rgba(255, 255, 255, 0);
}
a{
    text-decoration-line: none;
}
.header,
.header * {
  box-sizing: border-box;
}
.header {
  position: relative;
}
.header-2 {
  width: 1920px;
  height: 53px;
  position: static;
}
.frame-header-2 {
  background: rgba(255, 255, 255, 0);
  width: 1920px;
  height: 53px;
  position: absolute;
  left: 0px;
  top: 60px;
  overflow: hidden;
}
.frame-19 {
  display: flex;
  flex-direction: row;
  gap: 10px;
  align-items: flex-end;
  justify-content: center;
  width: 29px;
  height: 36px;
  position: absolute;
  left: 1573px;
  top: 17px;
}
.chek {
  color: #000000;
  text-align: center;
  font-family: "Inika-Bold", sans-serif;
  font-size: 36px;
  line-height: 41px;
  font-weight: 700;
  position: absolute;
  left: 356px;
  top: 60px;
  width: 140px;
  height: 53px;
  display: flex;
  align-items: center;
  justify-content: center;
}
.line-7 {
  border-style: solid;
  border-color: #000000;
  border-width: 4px 0 0 0;
  width: 850px;
  height: 0px;
  position: absolute;
  left: 540px;
  top: 113px;
  transform-origin: 0 0;
  transform: rotate(0deg) scale(1, 1);
}
.button-checkchek {
  padding: 10px;
  display: flex;
  flex-direction: row;
  gap: 10px;
  align-items: flex-end;
  justify-content: center;
  width: 50px;
  height: 50px;
  position: absolute;
  left: 1484px;
  top: 60px;
}
.frame-20 {
  display: flex;
  flex-direction: row;
  gap: 10px;
  align-items: flex-end;
  justify-content: center;
  flex-shrink: 0;
  width: 29px;
  height: 36px;
  position: relative;
  overflow: visible;
}
.button-totalsearch {
  padding: 0px 5px 0px 5px;
  display: flex;
  flex-direction: row;
  gap: 0px;
  align-items: center;
  justify-content: flex-start;
  height: 30px;
  position: absolute;
  left: 547px;
  top: 70px;
}
.div {
  color: #000000;
  text-align: center;
  font-family: "Inika-Bold", sans-serif;
  font-size: 20px;
  line-height: 41px;
  font-weight: 700;
  position: relative;
  width: 86px;
  height: 30px;
  display: flex;
  align-items: center;
  justify-content: center;
}
.totalsearchimg {
  flex-shrink: 0;
  width: 23.98px;
  height: 24px;
  position: relative;
  overflow: visible;
}
.button-search {
  padding: 10px;
  display: flex;
  flex-direction: row;
  gap: 10px;
  align-items: flex-end;
  justify-content: flex-start;
  width: 53px;
  height: 50px;
  position: absolute;
  left: 1337px;
  top: 60px;
}
.icon-search {
  flex-shrink: 0;
  width: 35.96px;
  height: 36px;
  position: relative;
  overflow: visible;
}
.button-mypage {
  padding: 10px;
  display: flex;
  flex-direction: row;
  gap: 10px;
  align-items: flex-end;
  justify-content: center;
  width: 50px;
  height: 50px;
  position: absolute;
  left: 1412px;
  top: 60px;
}
.icon-mypage {
  flex-shrink: 0;
  width: 36px;
  height: 36px;
  position: relative;
  overflow: visible;
}
.input-search {
  width: 669px;
  height: 50px;
  position: absolute;
  left: 668px;
  top: 60px;
  overflow: hidden;
}
.header-1 {
  width: 1920px;
  height: 60px;
  position: static;
}
.frame-header-1 {
  background: #ffffff;
  width: 1920px;
  height: 60px;
  position: absolute;
  left: 0px;
  top: 0px;
  backdrop-filter: blur(50000px);
}
.frame-18 {
  padding: 0px 10px 0px 10px;
  display: flex;
  flex-direction: row;
  gap: 20px;
  align-items: center;
  justify-content: center;
  height: 20px;
  position: absolute;
  left: 1200px;
  top: 23px;
}
.div2 {
  color: #000000;
  text-align: center;
  font-family: "Itim-Regular", sans-serif;
  font-size: 14px;
  line-height: 41px;
  font-weight: 400;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
}



</style>