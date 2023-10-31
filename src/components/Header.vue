<template>
   <header id="headerType" :class="['header__wrap', element]">
        <div class="header__inner">
            <div class="header__logo">
                <a href="#">green <em>site</em></a>
            </div>
            <nav class="header__menu">
                <ul>
                    <li><a href="#">헤더영역</a></li>
                    <li><a href="#">슬라이드 영역</a></li>
                    <li><a href="#">베너 영역</a></li>
                    <li><a href="#">컨텐츠 영역</a></li>
                    <li><a href="#">푸터 영역</a></li>
                </ul>
            </nav>
            <div class="header__member">
                <a href="#">로그인</a>
            </div>
        </div>
    </header>
</template>

<!-- props의 타입 정리 -->
<script>
    export default {
        props: {
            element: String,  
        }
    }
</script>