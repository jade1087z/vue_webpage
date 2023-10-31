<template>
    <section id="cardType" :class="['card__wrap', Element]">
        <h2>Green 사이트</h2>
        <p>
            웹디, 웹퍼블, 프론트엔드 개발자를 위한 사이트
        </p>
        <div class="card__inner container">
            <article class="card" v-for="(card, key) in cardInfo" :key="key">
                <figure class="card__header">
                    <img :src="card.img"  alt="card.title">
                </figure>
                <div class="card__body">
                    <h3 class="title">{{card.title}}</h3>
                    <p class="desc">{{card.desc}}</p>
                    <a href="/" class="btn">
                        자세히 보기
                        <span aria-hidden="true"><svg width="51" height="8" viewBox="0 0 51 8" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M50.3536 4.35355C50.5488 4.15829 50.5488 3.84171 50.3536 3.64645L47.1716 0.464466C46.9763 0.269204 46.6597 0.269204 46.4645 0.464466C46.2692 0.659728 46.2692 0.976311 46.4645 1.17157L49.2929 4L46.4645 6.82843C46.2692 7.02369 46.2692 7.34027 46.4645 7.53553C46.6597 7.7308 46.9763 7.7308 47.1716 7.53553L50.3536 4.35355ZM0 4.5H50V3.5H0V4.5Z" fill="black"/>
                            </svg>
                            </span>
                    </a>
                </div>
            </article>
           
        </div>
    </section>
</template>
<script>
    export default {
        props: {
            Element: String,
        },
        data: function () {
            return {
                cardInfo: [
                    {
                        img: "/src/assets/img/cardbg01.jpg",
                        title: "웹표준 사이트 만들기",
                        desc: "사이트를 만들기 위한 기초 강의",
                    },
                    {
                        img: "/src/assets/img/cardbg02.jpg",
                        title: "반응형 사이트 만들기",
                        desc: "사이트를 만들기 위한 기초 강의",
                    },
                    {
                        img: "/src/assets/img/cardbg03.jpg",
                        title: "페럴렉스 사이트 만들기",
                        desc: "사이트를 만들기 위한 기초 강의",
                    },
                ]
            }
        }
    }
</script>

<style>
.card__inner {
  display: flex;
  justify-content: space-between;
}
.card {
  width: 32%;
  background-color: #f5f5f5;
}
.card__header {
}
.card__body {
  padding: 24px;
}
.card__body .title {
  font-size: 24px;
  margin-bottom: 10px;
}
.card__body .desc {
  font-size: 18px;
  color: #666;
  line-height: 1.4;
  margin-bottom: 20px;
  font-weight: 300;

  /* 네줄 */
  overflow: hidden;
  text-overflow: ellipsis;
  display: -webkit-box;
  -webkit-line-clamp: 4;
  -webkit-box-orient: vertical;
}
.card__body .btn {
  color: #222;
}
</style>