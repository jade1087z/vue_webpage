<template>
    <footer id="footerType" :class="['footer__wrap', Element]">
        <h2 class="blind">풋터영역</h2>
        <div class="footer__inner container">
            <div class="footer__menu">
                <div>
                    <h3>사이트</h3>
                    <ul>
                        <li><a href="/">웹표준 사이트</a></li>
                        <li><a href="/">반응형 사이트</a></li>
                        <li><a href="/">페럴렉스 사이트</a></li>
                        <li><a href="/">포트폴리오 사이트</a></li>
                    </ul>
                </div>
                <div>
                    <h3>헤더유형</h3>
                    <ul>
                        <li><a href="/">웹표준 사이트</a></li>
                        <li><a href="/">반응형 사이트</a></li>
                    </ul>
                </div>
                <div>
                    <h3>슬라이드 유형</h3>
                    <ul>
                        <li><a href="/">웹표준 사이트</a></li>
                        <li><a href="/">반응형 사이트</a></li>
                    </ul>
                </div>
                <div>
                    <h3>이미지 유형</h3>
                    <ul>
                        <li><a href="/">웹표준 사이트</a></li>
                        <li><a href="/">반응형 사이트</a></li>
                    </ul>
                </div>
                <div>
                    <h3>카드 유형</h3>
                    <ul>
                        <li><a href="/">웹표준 사이트</a></li>
                        <li><a href="/">반응형 사이트</a></li>
                    </ul>
                </div>
                <div>
                    <h3>풋터 유형</h3>
                    <ul>
                        <li><a href="/">웹표준 사이트</a></li>
                        <li><a href="/">반응형 사이트</a></li>
                    </ul>
                </div>
            </div>
            <div class="footer__right">
                2023 Green <br />
                All right reseved
            </div>
        </div>
    </footer>
</template>

<script>
    export default {
        props: {
            Element: String,

        }
    }
</script>