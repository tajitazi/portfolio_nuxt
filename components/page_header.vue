<template>
  <nav class="navbar navbar-expand-md navbar-dark bg-dark sticky-top">
    <!-- サブコンポーネント -->
    <div class="container">
      <a class="navbar-brand" href="/">ポートフォリオ</a>
      <!-- 切り替えボタン -->
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbar-content"
        aria-controls="navbar-content"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon" />
      </button>
      <!-- ナビゲーション -->
      <div id="navbar-content" class="collapse navbar-collapse">
        <!-- ナビゲーションメニュー -->
        <!-- 左側メニュー：トップページの各コンテンツへのリンク -->
        <ul class="navbar-nav me-auto">
          <li class="nav-item active">
            <a class="nav-link" href="/about">Profile<span class="visually-hidden">(current)</span></a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/skill">Skill</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/work">Work</a>
          </li>
        </ul>
        <!-- 右側メニュー：お問い合わせページへのリンク -->
        <ul class="navbar-nav">
          <form class="d-flex">
            <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
            <button class="btn btn-outline-success" type="submit">
              Search
            </button>
          </form>
        </ul>
        <!-- /ナビゲーションメニュー -->
      </div>
    </div>
    <!-- /サブコンポーネント -->
  </nav>
</template>
