<template>
    <div>
        <header id="header">
            <section class="container">
                <h1 id="logo">
                    <a href="#" title="谷粒学院">
                        <img src="~/assets/img/logo.png" width="100%" alt="谷粒学院">
                    </a>
                </h1>
                <div class="h-r-nsl">
                    <ul class="nav">
                        <router-link to="/" tag="li" active-class="current" exact>
                            <a>首页</a>
                        </router-link>
                        <router-link to="/course" tag="li" active-class="current">
                            <a>课程</a>
                        </router-link>
                        <router-link to="/teacher" tag="li" active-class="current">
                            <a>名师</a>
                        </router-link>
                        <router-link to="/article" tag="li" active-class="current">
                            <a>文章</a>
                        </router-link>
                        <router-link to="/qa" tag="li" active-class="current">
                            <a>问答</a>
                        </router-link>
                    </ul>
                    <!-- / nav -->
                    <ul class="h-r-login">
                        <li id="no-login">
                            <a href="javascript:lrFun(1)" title="登录">
                                <em class="icon18 login-icon">&nbsp;</em>
                                <span class="vam ml5">登录</span>
                            </a>
                            |
                            <a href="javascript:lrFun(2)" title="注册">
                                <span class="vam ml5">注册</span>
                            </a>
                        </li>
                        <li class="mr10 undis" id="is-login-one">
                            <a href="#" title="消息" id="headerMsgCountId">
                                <em class="icon18 news-icon">&nbsp;</em>
                            </a>
                            <q class="red-point" style="display: none">&nbsp;</q>
                        </li>
                        <li class="h-r-user undis" id="is-login-two">
                            <a href="#" title>
                                <img
                                    src="~/assets/img/avatar-boy.gif"
                                    width="30"
                                    height="30"
                                    class="vam picImg"
                                    alt
                                >
                                <span class="vam disIb" id="userName"></span>
                            </a>
                            <a href="javascript:void(0)" title="退出" onclick="exit();" class="ml5">退出</a>
                        </li>
                        <!-- /未登录显示第1 li；登录后显示第2，3 li -->
                    </ul>
                    <aside class="h-r-search">
                        <form action="#" method="post">
                            <label class="h-r-s-box">
                                <input type="text" placeholder="输入你想学的课程" name="queryCourse.courseName" value>
                                <button type="submit" class="s-btn">
                                    <em class="icon18">&nbsp;</em>
                                </button>
                            </label>
                        </form>
                    </aside>
                </div>
                <aside class="mw-nav-btn">
                    <div class="mw-nav-icon"></div>
                </aside>
                <div class="clear"></div>
            </section>
        </header>
    </div>
</template>

<script>
export default {
    name: "Header"
}
</script>

<style scoped>

</style>