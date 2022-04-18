<template>
  <div class="profile">
    <Header />
    <main>
      <div class="container">
        <p class="border rounded-circle p-3" style="width: 100px;height: 100px;">
          正円にする場合
        </p>
        名前：田尻広人
        出身：千葉県
        年齢：33
        学歴：船橋情報ビジネス専門学校
        資格：基本情報技術者試験、HTML5レベル1、LPIC-1
      </div>
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/pageHeader.vue' // headerをインポート
import Footer from '@/components/pageFooter.vue' // footerをインポート

export default {
  name: 'IndexPage',
  components: {
    Header,
    Footer
  }
}
</script>
