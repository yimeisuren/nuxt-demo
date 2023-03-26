<template>

    <div>
        <Swiper/>

        <div id="aCoursesList">
            <HotClass/>
            <HotTeacher/>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            swiperOption: {
                //配置分页
                pagination: {
                    el: '.swiper-pagination'//分页的dom节点
                },
                //配置导航
                navigation: {
                    nextEl: '.swiper-button-next',//下一页dom节点
                    prevEl: '.swiper-button-prev'//前一页dom节点
                }
            }
        }
    }
}
</script>