<template>
    <section id="textType" :class="['text__wrap', Element]">
        <span>텍스트 유형</span>
        <h2>스크립트를 익히는 방법</h2>
        <div class="text__inner container">
            <div v-for="(text, key) in textInfo" :key = "key" :class="'text t' + (++key)">
                <h3 class="title">{{text.title}}</h3>
                <p class="desc">{{ text.desc }}</p>
                <a href="/" class="btn">{{text.btn}}</a>
            </div>
            
        </div>
    </section>
</template>

<script>
    export default {
        props: {
            Element: String
        },
        data: function () {
            return {
                    textInfo: [
                    {
                        title: "검색 이펙트",
                        desc: "자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다.",
                        btn: "더보기",
                    },
                    {
                        title: "검색 이펙트",
                        desc: "자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다.",
                        btn: "더보기",
                    },
                    {
                        title: "검색 이펙트",
                        desc: "자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다.",
                        btn: "더보기",
                    },
                    {
                        title: "검색 이펙트",
                        desc: "자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다.",
                        btn: "더보기",
                    },
                    {
                        title: "검색 이펙트",
                        desc: "자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다.",
                        btn: "더보기",
                    },
                    {
                        title: "검색 이펙트",
                        desc: "자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다.",
                        btn: "더보기",
                    },
                ]   
            }
        }
    }

</script>
<style>
.text__wrap {
}
.text__inner {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
.text {
  width: 32%;
  margin-bottom: 2%;
  padding: 20px;
  box-sizing: border-box;
  border-radius: 10px;
  transition: all 0.3s;
}
.text:hover {
  background-color: #f1f1f1;
}
.text .title {
  font-size: 24px;
  line-height: 1;
  margin-bottom: 10px;
  padding-top: 80px;
  position: relative;

  /* 한줄 */
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}
.text .title::before {
  content: '';
  position: absolute;
  left: 0;
  top: 0;
  width: 60px;
  height: 60px;
  background: url(../assets/img/text_icon.svg);
}
.text.t2 .title::before {
  background-position: -60px 0;
}
.text.t3 .title::before {
  background-position: -120px 0;
}
.text.t4 .title::before {
  background-position: -180px 0;
}
.text.t5 .title::before {
  background-position: -240px 0;
}
.text.t6 .title::before {
  background-position: -300px 0;
}
.text .desc {
  font-size: 18px;
  line-height: 1.4;
  margin-bottom: 20px;
  color: #666;

  /* 세줄 */
  overflow: hidden;
  text-overflow: ellipsis;
  display: -webkit-box;
  -webkit-line-clamp: 3;
  -webkit-box-orient: vertical;
}
.text .btn {
  line-height: 1;
  text-decoration: underline;
  text-underline-position: under;
  color: #666;
}
/* text */
</style>