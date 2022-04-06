<template>

    <div class="stock">
        <myheader :title="title"></myheader>
        <mt-navbar v-model="selected" class="tab" fixed>
            <mt-tab-item id="main">主流</mt-tab-item>
            <mt-tab-item id="hot">热门</mt-tab-item>
            <mt-tab-item id="close">我的收藏</mt-tab-item>
        </mt-navbar>
        <!-- tab-container -->
        <mt-tab-container v-model="selected">
            <mt-tab-container-item id="main">
                <!-- <header>沪深</header> -->
                <div class="hushen">
                    <!-- 指数板块 -->
<!--                    <div class="hushen-exponent clearfix">-->
<!--                        <div class="clearfix">-->
<!--                            <a href="javascrit:;">指数-->
<!--                                <span></span>-->
<!--                            </a>-->
<!--                        </div>-->
<!--                        <ul class="clearfix">-->
<!--                            <li>-->
<!--                                <router-link to="/stockDetails/stkCode=sh000001&stkName=上证指数">-->
<!--                                    <div>上证指数</div>-->
<!--                                    <div>3278.78</div>-->
<!--                                    <div><span>+10.23</span><span>+0.29%</span></div>-->
<!--                                </router-link>-->
<!--                            </li>-->
<!--                            <li>-->
<!--                                <a href="">-->
<!--                                    <div>深圳成指</div>-->
<!--                                    <div>10689.77</div>-->
<!--                                    <div><span>+75.69</span><span>+0.71%</span></div>-->
<!--                                </a>-->
<!--                            </li>-->
<!--                            <li>-->
<!--                                <a href="">-->
<!--                                    <div>创业板指</div>-->
<!--                                    <div>0.78%</div>-->
<!--                                    <div><span>+88.88</span><span>+0.24%</span></div>-->
<!--                                </a>-->
<!--                            </li>-->
<!--                        </ul>-->
<!--                    </div>-->
                    <!-- 领涨板块 -->
<!--                    <div class="hushen-plate clearfix">-->
<!--                        <div class="clearfix">-->
<!--                            <a href="javascrit:;">领涨板块-->
<!--                                 <span></span>-->
<!--                            </a>-->
<!--                        </div>-->
<!--                        <ul class="clearfix">-->
<!--                            <li>-->
<!--                                <a href="">-->
<!--                                    <div>养殖业</div>-->
<!--                                    <div>0.98%</div>-->
<!--                                    <div><span>牧原股份</span><span>+0.44%</span></div>-->
<!--                                </a>-->
<!--                            </li>-->
<!--                            <li>-->
<!--                                <a href="">-->
<!--                                    <div>农业服务</div>-->
<!--                                    <div>0.85%</div>-->
<!--                                    <div><span>伟康生化</span><span>+0.14%</span></div>-->
<!--                                </a>-->
<!--                            </li>-->
<!--                            <li>-->
<!--                                <a href="">-->
<!--                                    <div>新材料</div>-->
<!--                                    <div>0.78%</div>-->
<!--                                    <div><span>正海磁材</span><span>+0.24%</span></div>-->
<!--                                </a>-->
<!--                            </li>-->
<!--                            <li>-->
<!--                                <a href="">-->
<!--                                    <div>保险及其他</div>-->
<!--                                    <div>0.72%</div>-->
<!--                                    <div><span>中国平安</span><span>+0.34%</span></div>-->
<!--                                </a>-->
<!--                            </li>-->
<!--                            <li>-->
<!--                                <a href="">-->
<!--                                    <div>养殖业</div>-->
<!--                                    <div>0.98%</div>-->
<!--                                    <div><span>牧原股份</span><span>+0.44%</span></div>-->
<!--                                </a>-->
<!--                            </li>-->
<!--                            <li>-->
<!--                                <a href="">-->
<!--                                    <div>养殖业</div>-->
<!--                                    <div>0.98%</div>-->
<!--                                    <div><span>牧原股份</span><span>+0.44%</span></div>-->
<!--                                </a>-->
<!--                            </li>-->
<!--                        </ul>-->
<!--                    </div>-->
                    <!-- 榜单模块 -->
                    <div class="listModule">
                        <yd-accordion accordion>
                            <yd-accordion-item title="涨幅榜" open>
                                <!-- <div style="padding: .24rem;">
                                    涨幅榜
                                </div> -->
                                <ul>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                </ul>
                            </yd-accordion-item>
                            <yd-accordion-item title="跌幅榜">
                                <!-- <div style="padding: .24rem;">
                                    涨幅榜
                                </div> -->
                                <ul>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                </ul>
                            </yd-accordion-item>
                            <yd-accordion-item title="换手率榜">
                                <!-- <div style="padding: .24rem;">
                                    涨幅榜
                                </div> -->
                                <ul>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                </ul>
                            </yd-accordion-item>
                            <yd-accordion-item title="量比榜">
                                <!-- <div style="padding: .24rem;">
                                    涨幅榜
                                </div> -->
                                <ul>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                </ul>
                            </yd-accordion-item>
                            <yd-accordion-item title="成交额榜">
                                <!-- <div style="padding: .24rem;">
                                    涨幅榜
                                </div> -->
                                <ul>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                </ul>
                            </yd-accordion-item>
                        </yd-accordion>
                    </div>
                </div>
            </mt-tab-container-item>
            <mt-tab-container-item id="hot">
                <!-- <header>沪深</header> -->
                <div class="hushen">
                    <!-- 指数板块 -->
                    <div class="hushen-exponent clearfix">
                        <div class="clearfix">
                            <a href="javascrit:;">指数
                                <span></span>
                            </a>
                        </div>
                        <ul class="clearfix">
                            <li>
                                <router-link to="/stockDetails/stkCode=sh000001&stkName=上证指数">
                                    <div>上证指数</div>
                                    <div>3278.78</div>
                                    <div><span>+10.23</span><span>+0.29%</span></div>
                                </router-link>
                            </li>
                            <li>
                                <a href="">
                                    <div>深圳成指</div>
                                    <div>10689.77</div>
                                    <div><span>+75.69</span><span>+0.71%</span></div>
                                </a>
                            </li>
                            <li>
                                <a href="">
                                    <div>创业板指</div>
                                    <div>0.78%</div>
                                    <div><span>+88.88</span><span>+0.24%</span></div>
                                </a>
                            </li>
                        </ul>
                    </div>
                    <!-- 领涨板块 -->
                    <div class="hushen-plate clearfix">
                        <div class="clearfix">
                            <a href="javascrit:;">领涨板块
                                 <span></span>
                            </a>
                        </div>
                        <ul class="clearfix">
                            <li>
                                <a href="">
                                    <div>养殖业</div>
                                    <div>0.98%</div>
                                    <div><span>牧原股份</span><span>+0.44%</span></div>
                                </a>
                            </li>
                            <li>
                                <a href="">
                                    <div>农业服务</div>
                                    <div>0.85%</div>
                                    <div><span>伟康生化</span><span>+0.14%</span></div>
                                </a>
                            </li>
                            <li>
                                <a href="">
                                    <div>新材料</div>
                                    <div>0.78%</div>
                                    <div><span>正海磁材</span><span>+0.24%</span></div>
                                </a>
                            </li>
                            <li>
                                <a href="">
                                    <div>保险及其他</div>
                                    <div>0.72%</div>
                                    <div><span>中国平安</span><span>+0.34%</span></div>
                                </a>
                            </li>
                            <li>
                                <a href="">
                                    <div>养殖业</div>
                                    <div>0.98%</div>
                                    <div><span>牧原股份</span><span>+0.44%</span></div>
                                </a>
                            </li>
                            <li>
                                <a href="">
                                    <div>养殖业</div>
                                    <div>0.98%</div>
                                    <div><span>牧原股份</span><span>+0.44%</span></div>
                                </a>
                            </li>
                        </ul>
                    </div>
                    <!-- 榜单模块 -->
                    <div class="listModule">
                        <yd-accordion accordion>
                            <yd-accordion-item title="涨幅榜" open>
                                <!-- <div style="padding: .24rem;">
                                    涨幅榜
                                </div> -->
                                <ul>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                </ul>
                            </yd-accordion-item>
                            <yd-accordion-item title="跌幅榜">
                                <!-- <div style="padding: .24rem;">
                                    涨幅榜
                                </div> -->
                                <ul>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                </ul>
                            </yd-accordion-item>
                            <yd-accordion-item title="换手率榜">
                                <!-- <div style="padding: .24rem;">
                                    涨幅榜
                                </div> -->
                                <ul>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                </ul>
                            </yd-accordion-item>
                            <yd-accordion-item title="量比榜">
                                <!-- <div style="padding: .24rem;">
                                    涨幅榜
                                </div> -->
                                <ul>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                </ul>
                            </yd-accordion-item>
                            <yd-accordion-item title="成交额榜">
                                <!-- <div style="padding: .24rem;">
                                    涨幅榜
                                </div> -->
                                <ul>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                </ul>
                            </yd-accordion-item>
                        </yd-accordion>
                    </div>
                </div>
            </mt-tab-container-item>
            <mt-tab-container-item id="close">
                <!-- <header>沪深</header> -->
                <div class="hushen">
                    <!-- 指数板块 -->
                    <div class="hushen-exponent clearfix">
                        <div class="clearfix">
                            <a href="javascrit:;">指数
                                <span></span>
                            </a>
                        </div>
                        <ul class="clearfix">
                            <li>
                                <router-link to="/stockDetails/stkCode=sh000001&stkName=上证指数">
                                    <div>上证指数</div>
                                    <div>3278.78</div>
                                    <div><span>+10.23</span><span>+0.29%</span></div>
                                </router-link>
                            </li>
                            <li>
                                <a href="">
                                    <div>深圳成指</div>
                                    <div>10689.77</div>
                                    <div><span>+75.69</span><span>+0.71%</span></div>
                                </a>
                            </li>
                            <li>
                                <a href="">
                                    <div>创业板指</div>
                                    <div>0.78%</div>
                                    <div><span>+88.88</span><span>+0.24%</span></div>
                                </a>
                            </li>
                        </ul>
                    </div>
                    <!-- 领涨板块 -->
                    <div class="hushen-plate clearfix">
                        <div class="clearfix">
                            <a href="javascrit:;">领涨板块
                                 <span></span>
                            </a>
                        </div>
                        <ul class="clearfix">
                            <li>
                                <a href="">
                                    <div>养殖业</div>
                                    <div>0.98%</div>
                                    <div><span>牧原股份</span><span>+0.44%</span></div>
                                </a>
                            </li>
                            <li>
                                <a href="">
                                    <div>农业服务</div>
                                    <div>0.85%</div>
                                    <div><span>伟康生化</span><span>+0.14%</span></div>
                                </a>
                            </li>
                            <li>
                                <a href="">
                                    <div>新材料</div>
                                    <div>0.78%</div>
                                    <div><span>正海磁材</span><span>+0.24%</span></div>
                                </a>
                            </li>
                            <li>
                                <a href="">
                                    <div>保险及其他</div>
                                    <div>0.72%</div>
                                    <div><span>中国平安</span><span>+0.34%</span></div>
                                </a>
                            </li>
                            <li>
                                <a href="">
                                    <div>养殖业</div>
                                    <div>0.98%</div>
                                    <div><span>牧原股份</span><span>+0.44%</span></div>
                                </a>
                            </li>
                            <li>
                                <a href="">
                                    <div>养殖业</div>
                                    <div>0.98%</div>
                                    <div><span>牧原股份</span><span>+0.44%</span></div>
                                </a>
                            </li>
                        </ul>
                    </div>
                    <!-- 榜单模块 -->
                    <div class="listModule">
                        <yd-accordion accordion>
                            <yd-accordion-item title="涨幅榜" open>
                                <!-- <div style="padding: .24rem;">
                                    涨幅榜
                                </div> -->
                                <ul>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                </ul>
                            </yd-accordion-item>
                            <yd-accordion-item title="跌幅榜">
                                <!-- <div style="padding: .24rem;">
                                    涨幅榜
                                </div> -->
                                <ul>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                </ul>
                            </yd-accordion-item>
                            <yd-accordion-item title="换手率榜">
                                <!-- <div style="padding: .24rem;">
                                    涨幅榜
                                </div> -->
                                <ul>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                </ul>
                            </yd-accordion-item>
                            <yd-accordion-item title="量比榜">
                                <!-- <div style="padding: .24rem;">
                                    涨幅榜
                                </div> -->
                                <ul>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                </ul>
                            </yd-accordion-item>
                            <yd-accordion-item title="成交额榜">
                                <!-- <div style="padding: .24rem;">
                                    涨幅榜
                                </div> -->
                                <ul>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                    <li>
                                        <div><span>N出版</span><span>6000001</span><span>新</span></div>
                                        <div>4.88</div>
                                        <div>+44.99%</div>
                                    </li>
                                </ul>
                            </yd-accordion-item>
                        </yd-accordion>
                    </div>
                </div>
            </mt-tab-container-item>
        </mt-tab-container>
    </div>
</template>
<script>
import myheader from './header.vue'
import banner from "./banner";

export default {
  name: 'stategy',
  data() {
    return {
      // title: '君弘策略'
      selected: 'main',
      title: '行情'
    };
  },
  computed: {},
  watch: {},
  components: {
    myheader,
    banner
  }
};

</script>
<style>
.hushen-exponent {
  padding-right: 0.938rem;
  padding-left: 0.938rem;
  margin-bottom: 0.3125rem;
  background-color: #fff;
}

</style>
