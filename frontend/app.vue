<template>
  <div class="root">
    <nav class="w-screen h-20 border-b-2 flex items-center">
      <Icon name="uil:github" class="flex items-center ml-5" />
      <div class="tab flex-auto flex justify-end">
        <a href="" v-for="(tab, i) in tabs" :key="i">{{ tab }}</a>
      </div>
    </nav>
    <main>
      <div class="box-1 flex flex-col w-full">
        <div class="subscribe">모두를 위한 동아리 동아리 관리 플랫폼</div>
        <hr class="line" style="border: 1px white solid; width: 180px" />
        <div class="small-box flex justify-around items-center w-full h-full">
          <div class="card">진호가 만들었어요</div>
          <div class="card">재헌이가 만들었어요</div>
          <div class="card">상헌이가 만들었어요</div>
          <div class="card">재흠이가 만들었어요</div>
        </div>
      </div>
      <div class="box-2 flex flex-col w-full"></div>
      <div class="box-3 flex flex-col w-full"></div>
    </main>
  </div>
  <footer>
    <div class="logo"></div>
    <div class="footer-box">
      <div class="copyright">
        <p class="addr">서울특별시 성동구 왕십리로 222 경제금융관 506호</p>
        <p class="tel">02.2220.1807</p>
        <p class="copy">COPYRIGHT ⓒ 2023 ZINOZZING. ALL RIGHTS RESERVED.</p>
      </div>
    </div>
    <div class="site"></div>
  </footer>
</template>
<script>
export default {
  data() {
    return {
      tabs: [
        "게시판",
        "회계내역확인",
        "설문조사",
        "실시간채팅",
        "회원관리",
        "회원가입/로그인",
      ],
    };
  },
};
</script>
<style>
.root {
  display: flex;
  flex-direction: column;
  min-height: 350vh;
}

.tab {
  padding: 15px;
  border-radius: 5px;
}
.tab a {
  padding: 10px;
  text-decoration: none;
}

nav {
  position: sticky;
  top: 0;
  background-color: white;
}

.box-1 {
  height: 75vh;
  color: white;
  background-color: #8bc6ec;
  background-image: linear-gradient(135deg, #8bc6ec 0%, #9599e2 100%);
}

.box-2 {
  height: 75vh;
}

.box-3 {
  height: 75vh;
  background-color: black;
}

.box-4 {
  height: 75vh;
  background-color: white;
}

.subscribe {
  padding: 80px 0 0 5%;
  font-size: 40px;
  font-weight: 700;
}

.line {
  margin-left: 5%;
}

.card {
  font-size: 25px;
}

footer {
  width: 100%;
  height: 15vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  color: #666666;
  background-color: #2c2d30;
  font-size: small;
  position: relative;
}

.footer-box {
  display: flex;
  text-align: center;
}
</style>
