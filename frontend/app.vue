<template>
  <div>
    <header class="w-screen h-24 border-b-2 flex items-center">
      <Icon name="uil:github" class="flex items-center ml-5" />
      <div class="tab flex-auto flex justify-end">
        <a href="" v-for="(tab, i) in tabs" :key="i">{{ tab }}</a>
      </div>
    </header>
    <nav></nav>
    <main></main>
    <footer></footer>
  </div>
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
.tab {
  padding: 15px;
  border-radius: 5px;
}
.tab a {
  padding: 10px;
  text-decoration: none;
}
</style>
