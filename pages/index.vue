<template>
  <div class="home">
    <Header />
    <main>
      <!-- メインビジュアル -->
      <div class="py-4">
        <div class="container">
          <!-- カルーセル外枠 -->
          <div id="main_visual" class="carousel slide">
            <!-- カルーセル内枠 -->
            <carousel
              :per-page="1"
              :autoplay="true"
              :autoplay-timeout="3000"
              :loop="true"
              :speed="500"
              :navigation-enabled="true"
              navigation-prev-label="〈"
              navigation-next-label="〉"
            >
              <!-- スライド01 -->
              <slide>
                <img class="img-fluid" src="~assets/slide_01.jpg" alt="1枚目画像">
                <div class="carousel-caption d-none d-md-block">
                  <h2>ポートフォリオサイト作りました</h2>
                  <p>説明欄</p>
                </div>
              </slide>
              <!-- / スライド01 -->
              <!-- スライド02 -->
              <slide>
                <img class="img-fluid" src="~assets/slide_02.jpg" alt="2枚目画像">
                <div class="carousel-caption d-none d-md-block">
                  <h2>ポートフォリオサイト作りました</h2>
                  <p>説明欄</p>
                </div>
              </slide>
              <!-- / スライド02 -->
              <!-- スライド03 -->
              <slide>
                <img class="img-fluid" src="~assets/slide_03.jpg" alt="3枚目画像">
                <div class="carousel-caption d-none d-md-block">
                  <h2>ポートフォリオサイト作りました</h2>
                  <p>説明欄</p>
                </div>
              </slide>
              <!-- / スライド03 -->
            </carousel>
            <!-- / カルーセル内側 -->
          </div>
          <!-- / カルーセル -->
        </div>
      </div>
      <!-- / メインビジュアル -->
      <!-- /コンテンツ01 -->
      <div class="py-4 bg-light">
        <section id="topPage">
          <div class="container">
            <!-- 上段 -->
            <div class="row mb-4">
              <div class="col-md-12 mb-3">
                <h3 class="mb-3">
                  ポートフォリオタイトル
                </h3>
                <p>このポートフォリオでは、私のプロフィール・スキル・業務経歴についてまとめさせていただきました。</p>
              </div>
            </div>
            <!-- /上段 -->
            <!-- 下段 -->
            <div class="row">
              <div class="col-md-4">
                <div class="card mb-3">
                  <a href="/ProfilePage">
                    <img src="~assets/profile_top.png" alt="Profile" class="img-fluid">
                  </a>
                  <div class="card-body d-flex justify-content-between">
                    <h4 class="card-title">
                      Profile
                    </h4>
                  </div>
                </div>
              </div>
              <div class="col-md-4">
                <div class="card mb-3">
                  <a href="/skillPage">
                    <img src="../assets/skill_top.png" alt="Skill" class="img-fluid">
                    <div class="card-body d-flex justify-content-between">
                      <h4 class="card-title">
                        Skill
                      </h4>
                    </div>
                  </a>
                </div>
              </div>
              <div class="col-md-4">
                <div class="card mb-3">
                  <a href="/workPage">
                    <img src="~assets/work_top.png" alt="Work" class="img-fluid">
                  </a>
                  <div class="card-body d-flex justify-content-between">
                    <h4 class="card-title">
                      Work
                    </h4>
                  </div>
                </div>
              </div>
            </div>
            <!-- /下段 -->
          </div>
        </section>
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
