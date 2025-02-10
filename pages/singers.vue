<template>
  <div class="singers-page" :style="{ backgroundColor: '#1f75fe', color: 'white', textAlign: 'center', padding: '50px' }">
    <h1>Singer Introductions</h1>
    <ul class="singers-list" :style="{ listStyle: 'none', padding: '0' }">
      <li v-for="(singer, index) in singers" :key="index" class="singer-item" :style="{ display: 'flex', alignItems: 'center', marginBottom: '20px', padding: '10px', backgroundColor: 'white', color: '#333', borderRadius: '10px' }">
        <img :src="require(`~/assets/image/${singer.image}`)" alt="singer" class="singer-image" :style="{ width: 'auto', height: 'auto', objectFit: 'cover', borderRadius: 'auto', marginRight: 'auto' }" />
        <div class="singer-info" :style="{ display: 'flex', flexDirection: 'column' }">
          <span class="singer-name" :style="{ fontSize: '55px', fontWeight: 'bold' }">{{ singer.name }}</span>
          <span class="singer-song" :style="{ fontSize: '35px', color: '#888' }">{{ singer.song }}</span>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "SingersPage",
  data() {
    return {
      singers: [
        { name: "秋川雅史", song: "千の風になって", image: "Akikawa.jpeg" },
        { name: "安室奈美恵", song: "Can You Celebrate", image: "Amuro.jpeg" },
        { name: "絢香", song: "三日月", image: "Ayaka.jpeg" },
        { name: "嵐", song: "A・RA・SHI", image: "Arashi.jpeg" },
        { name: "アンジェラ・アキ", song: "手紙〜拝啓 十五の君へ〜", image: "Anjera.jpeg" },
        { name: "家入レオ", song: "君がくれた夏", image: "Ieiri.jpeg" },
        { name: "いきものがかり", song: "YELL", image: "Ikimono.jpeg" },
        { name: "石井竜也", song: "浪漫飛行", image: "Ishii.jpeg" },
        { name: "大黒摩季", song: "ら・ら・ら", image: "Ooguro.jpeg" },
        { name: "大塚愛", song: "さくらんぼ", image: "Ootsuka.jpeg" },
        { name: "コブクロ", song: "蕾", image: "Kobukuro.jpeg" },
        { name: "倖田來未", song: "愛のうた", image: "Koda.jpeg" },
        { name: "倉木麻衣", song: "Secret of my heart", image: "Kuraki.jpeg" },
        { name: "桑田佳祐", song: "明日晴れるかな", image: "Kuwata.jpeg" },
        { name: "AI", song: "ハピネス", image: "Ai.jpeg" },
        { name: "Aiko", song: "カブトムシ", image: "Aiko.jpeg" },
        { name: "AKB48", song: "ヘビーローテーション", image: "AKB.jpeg" },
        { name: "Aqua Timez", song: "虹", image: "Aqua.jpeg" },
        { name: "Every Little Thing", song: "Time goes by", image: "Every.jpeg" },
        { name: "EXILE", song: "Choo Choo Train", image: "Exile.jpeg" },
        { name: "THE ALFEE", song: "星空の下のディスタンス", image: "The.jpeg" },
      ]
    };
  }
};
</script>