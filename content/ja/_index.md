---
featured_image: '/img/title.png'
description: 'クレストンホーム杯 公式サイト'
---

<!-- jQuery.jsの読み込み -->
  <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.3.2/jquery.min.js"></script>

  <!-- スムーズスクロール部分の記述 -->
  <script>
  $(function(){
   // #で始まるアンカーをクリックした場合に処理
   $('a[href^=#]').click(function() {
      // スクロールの速度
      var speed = 100; // ミリ秒
      // アンカーの値取得
      var href= $(this).attr("href");
      // 移動先を取得
      var target = $(href == "#" || href == "" ? 'html' : href);
      // 移動先を数値で取得
      var position = target.offset().top;
      // スムーススクロール
      $('body,html').animate({scrollTop:position}, speed, 'swing');
      return false;
    });
  });
  </script>

{{< nav_box page="home" >}}
