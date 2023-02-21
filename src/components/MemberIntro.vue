<template>
    <div class="mt-32 px-4 max-w-[920px] mx-auto">
        <div class="big-title text-center py-16">
            <p>團隊介紹</p>
        </div>
        <div class="block-content text-[18px] tracking-[5px] max-w-[920px] mx-auto text-justify">
            <div>
                <div class="flex items-center gap-5">
                    <p class="px-4 py-2 bg-[#968E85] text-white font-semibold rounded-[3px]">手建築姐</p>
                    <p class="text-[#968E85] font-semibold text-[20px]">Sylvia</p>
                </div>
                <p class="mt-[40px] text-base">把建築輕鬆帶過，顯然並不適合。
                    我們不得不面對一個非常尷尬的事實，那就是，若發現問題比我們想像的還要深奧，那肯定不簡單。帶著這些問題，我們一起來審視建築。儘管如此，別人往往卻不這麼想。透過逆向歸納，得以用最佳的策略去分析建築。
                </p>
                <div class="flex flex-wrap md:flex-nowrap  items-start justify-between gap-10 md:gap-[100px] mt-4">
                    <div>
                        <p class="text-base">
                            建築改變了我的命運。建築，到底應該如何實現。問題的核心究竟是什麼？契訶夫說過一句經典的名言，蚜蟲吃青草，銹吃鐵，虛偽吃靈魂。這讓我對於看待這個問題的方法有了巨大的改變。</p>
                        <img class="mt-4 ml-auto" src="@/assets/images/sign_wang.png" alt="">
                    </div>
                    <div
                        class="w-[400px] sm:ml-auto flex flex-col gap-0.5 border-l-[5px] border-[#D9D9D9] pl-[16px] py-1">
                        <div
                            class="w-full flex items-center justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px] ">
                            <div class="w-[70px] md:w-[110px] flex  justify-between shrink-0">
                                <p>2023- </p>
                                <p class="mr-[-0.025em] md:mr-[-5px]">至今</p>
                            </div>
                            <p class="ml-4">手建築有限公司 Founder</p>
                        </div>
                        <div
                            class="w-full flex items-center justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                            <div class="w-[70px] md:w-[110px] flex justify-between shrink-0">
                                <p>2021- </p>
                                <p class="mr-[-0.025em] md:mr-[-5px]">至今</p>
                            </div>
                            <p class="ml-4">前端網頁設計師</p>
                        </div>
                        <div
                            class="w-full flex items-center justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                            <div class="w-[70px] md:w-[110px] flex justify-between shrink-0">
                                <p>2019-</p>
                                <p>2021</p>
                            </div>
                            <p class="ml-4">北科互動設計系 碩士</p>
                        </div>
                        <div
                            class="w-full flex items-center justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                            <div class="w-[70px] md:w-[110px] flex justify-between shrink-0">
                                <p>2016-</p>
                                <p>2019</p>
                            </div>
                            <p class="ml-4">南臺創新產品設計系 學士</p>
                        </div>
                    </div>
                </div>

                <div class="w-full md:flex justify-end mt-10 text-base">
                    <div class="bubble  flex items-center justify-center"
                        :class="[clientWidth < 770 ? 'bubble-bottom' : 'bubble-right']">
                        <p class="text-sm">一棟住宅的結構安全取決於是否有完善並且公開透明的施工品質。</p>
                    </div>
                    <div>
                        <img class="w-[200px] h-[200px] ml-auto" src="@/assets/images/avatar_wang.png" alt="">
                        <div class="w-[300px] ml-auto flex flex-col items-end px-5">
                            <p
                                class="bg-[#CABFB3] text-sm  tracking-[2.5px] mr-[-2.5px] rounded-sm text-[white] inline-block px-1.5">
                                手建築有限公司</p>
                            <div class="mt-2 flex items-end gap-12">
                                <div class="">
                                    <p class="text-[#756C62] text-[13px] tracking-[5px]">共同創辦人</p>
                                    <p class="mt-[-6px] text-[#968E85] text-[12px] tracking-[1px]">CO-FOUNDER</p>
                                </div>
                                <div class="text-right">
                                    <p class="text-[24px] text-[#3C3C3C]">王雅智</p>
                                    <p class="text-[#979797] text-xs mt-1.5 tracking-[2.5px]">Ya-Chih Wang</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
        <div class="mt-32 block-content text-[18px] tracking-[5px] max-w-[920px] mx-auto text-justify">
            <div class="flex items-center gap-5">
                <p class="px-4 py-2 bg-[#968E85] text-white font-semibold rounded-[3px]">手建築哥</p>
                <p class="text-[#968E85] font-semibold text-[20px]">田桑</p>
            </div>
            <div class="mt-[40px] text-base flex flex-wrap md:flex-nowrap items-start gap-8">
                <div>
                    <div>
                        就我個人來說，建築對我的意義，不能不說非常重大。既然，我們都知道，只要有意義，那麼就必須慎重考慮。看看別人，再想想自己，會發現問題的核心其實就在你身旁。塞內加說過一句很有意思的話，肚子是聽不進勸告的。這似乎解答了我的疑惑。
                    </div>
                    <div class="mt-[17px]">
                        其實，若思緒夠清晰，那麼建築也就不那麼複雜了。帕納說過，陳舊的眼光感受不了任何新景像。這段話的餘韻不斷在我腦海中迴盪著。建築絕對是史無前例的。我們普遍認為，若能理解透徹核心原理，對其就有了一定的了解程度。當你搞懂後就會明白了。一般來講，我們都必須務必慎重的考慮考慮。深入的探討建築，是釐清一切的關鍵。
                    </div>
                    <img class="mt-4 ml-auto" src="@/assets/images/sign_wang.png" alt="">
                </div>
                <div class=" w-full md:w-autp border-l-[5px] border-[#D9D9D9] pl-[16px] flex flex-col gap-[2px]">
                    <div
                        class="w-full flex items-center gap-[15px] justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                        <p>2023</p>
                        <p>手建築有限公司 Founder</p>
                    </div>
                    <div
                        class="w-full flex items-center gap-[15px] justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                        <p>2021</p>
                        <p>成大單車節教育論壇 講者</p>
                    </div>
                    <div
                        class="w-full flex items-center gap-[15px] justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                        <p>2021</p>
                        <p>成大College X 密集式課程 講師</p>
                    </div>
                    <div
                        class="w-full flex items-center gap-[15px] justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                        <p>2020</p>
                        <p>教育部青年迴響計畫 南區講者</p>
                    </div>
                    <div
                        class="w-full flex items-center gap-[15px] justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                        <p>2019</p>
                        <p>進化學院 Founder</p>
                    </div>
                    <div
                        class="w-full flex items-center gap-[15px] justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                        <p>2019</p>
                        <p>醫療器材集團 銷售顧問</p>
                    </div>
                    <div
                        class="w-full flex items-center gap-[15px] justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                        <p>2018</p>
                        <p>台灣50大集團 簡報講師</p>
                    </div>
                    <div
                        class="w-full flex items-center gap-[15px] justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                        <p>2017</p>
                        <p>婚禮主持人</p>
                    </div>
                    <div
                        class="w-full flex items-center gap-[15px] justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                        <p>2017</p>
                        <p>高中韓文代課</p>
                    </div>
                    <div
                        class="w-full flex items-center gap-[15px] justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                        <p>2016</p>
                        <p>擴增實境 / 虛擬實境研發工程師</p>
                    </div>
                    <div
                        class="w-full flex items-center gap-[15px] justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                        <p>2015</p>
                        <p>中華民國陸軍空降特戰部隊</p>
                    </div>
                    <div
                        class="w-full flex items-center gap-[15px] justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                        <p>2014</p>
                        <p>成大資訊工程畢</p>
                    </div>
                </div>
            </div>
            <div class="text-base">
                <div class="w-full md:flex justify-start mt-10 ">
                    <img class="w-[200px] h-[200px] " src="@/assets/images/avatar_tiang.png" alt="">
                    <div class="bubble  flex items-center justify-center"
                        :class="[clientWidth < 770 ? 'bubble-top' : 'bubble-left']">
                        <p class="text-sm">一棟住宅的結構安全取決於是否有完善並且公開透明的施工品質。</p>
                    </div>
                </div>
                <div class="w-[320px] flex flex-col items-start px-5 mt-10 md:mt-0">
                    <p
                        class="bg-[#CABFB3] text-sm tracking-[2.5px] mr-[-2.5px] rounded-sm text-[white] inline-block px-1.5">
                        手建築有限公司</p>
                    <div class="mt-2 flex items-end gap-20">
                        <div class="">
                            <p class="text-[#756C62] text-[13px] tracking-[5px]">創辦人</p>
                            <p class="mt-[-6px] text-[#968E85] text-[12px] tracking-[1px]">FOUNDER</p>
                        </div>
                        <div class="text-left">
                            <p class="text-[24px] text-[#3C3C3C]">田烜睿</p>
                            <p class="text-[#979797] text-xs mt-1.5 tracking-[2.5px]">Xuan-Ray Tiang</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="mt-32 block-content text-[18px] tracking-[5px] max-w-[920px] mx-auto text-justify">
            <div class="flex items-center gap-5">
                <p class="px-4 py-2 bg-[#968E85] text-white font-semibold rounded-[3px]">手建築老爹</p>
                <p class="text-[#968E85] font-semibold text-[20px]">葉總</p>
            </div>
            <div class="mt-[40px] text-base">
                <p>購屋者如果購地自建，在台灣，只要再申請建設公司的營業登記，就可以將自建屋的行為，宣佈自己為建商。</p>
                <div class="mt-4 flex flex-wrap md:flex-nowrap items-start gap-8">
                    <div>
                        <div>
                            <p>差別就只是一個 ——「營業登記」。</p>
                            <p class="mt-4">當然，後續的設計、營造，才是建商和購屋者真正的差異，購屋者不懂的設計和如何蓋房子，建商卻很清楚。<br />沒錯，所以購屋者才需要我們的幫忙。</p>
                            <p class="mt-4">我們是什麼公司？<br />擔任建商角色的顧問公司——提供和協助購屋者當建商的所有專業。</p>
                            <p class="mt-4">我們就是要協助做到跟建商比要低於建商售價的四成，而且已經包含我們的顧問費。</p>
                        </div>
                        <img class="mt-4 ml-auto" src="@/assets/images/sign_wang.png" alt="">
                    </div>
                    <div
                        class="w-[460px] sm:ml-auto flex flex-col gap-0.5 border-l-[5px] border-[#D9D9D9] pl-[16px] py-1 whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                        <div class="w-full flex items-center justify-between text-[#968E85] ">
                            <div class="w-[70px] md:w-[110px] flex  justify-between shrink-0">
                                <p>2023- </p>
                                <p class="mr-[-0.025em] md:mr-[-5px]">至今</p>
                            </div>
                            <p class="ml-4">凱元土木包工業 技術顧問</p>
                        </div>
                        <div class="w-full flex items-center justify-between text-[#968E85]">
                            <div class="w-[70px] md:w-[110px] flex justify-between shrink-0">
                                <p>1999-</p>
                                <p class="mr-[-0.025em] md:mr-[-5px]">2022</p>
                            </div>
                            <p class="ml-4">睿的事業有限公司 總經理</p>
                        </div>
                        <p class="text-[#CABFB3] text-end">（總共完成設計、營造上百棟的客製化私人住宅）</p>
                        <div class="w-full flex items-center justify-between text-[#968E85]">
                            <div class="w-[70px] md:w-[110px] flex justify-between shrink-0">
                                <p>1997-</p>
                                <p>1998</p>
                            </div>
                            <p class="ml-4">鄉林建設 副總經理</p>
                        </div>
                        <p class="text-[#CABFB3] text-end">（鄉林集團涵碧樓飯店設計行銷諮詢）</p>
                        <div class="w-full flex items-center justify-between text-[#968E85]">
                            <div class="w-[70px] md:w-[110px] flex justify-between shrink-0">
                                <p></p>
                                <p>1996</p>
                            </div>
                            <p class="ml-4">中國生產力中心 雲嘉南工地管理講師</p>
                        </div>
                        <div class="w-full flex items-center justify-between text-[#968E85]">
                            <div class="w-[70px] md:w-[110px] flex justify-between shrink-0">
                                <p>1993-</p>
                                <p>1997</p>
                            </div>
                            <p class="ml-4">力百營造有限公司 副總經理</p>
                        </div>
                        <div class="w-full flex items-center justify-between text-[#968E85]">
                            <div class="w-[70px] md:w-[110px] flex justify-between shrink-0">
                                <p>1993-</p>
                                <p>1997</p>
                            </div>
                            <p class="ml-4">瑞銘建設、築福事業有限公司 總經理</p>
                        </div>
                        <div class="w-full flex items-center justify-between text-[#968E85]">
                            <div class="w-[70px] md:w-[110px] flex justify-between shrink-0">
                                <p>1990-</p>
                                <p>1993</p>
                            </div>
                            <p class="ml-4">南紡集團南紡建設 專業經理人</p>
                        </div>
                        <div class="w-full flex items-center justify-between text-[#968E85]">
                            <div class="w-[70px] md:w-[110px] flex justify-between shrink-0">
                                <p>1987-</p>
                                <p>1990</p>
                            </div>
                            <p class="ml-4">宗欣建設集團宗揚房屋 副總經理</p>
                        </div>
                        <div class="w-full flex items-start justify-between text-[#968E85]">
                            <div class="w-[70px] md:w-[110px] flex justify-between shrink-0">
                                <p>1983-</p>
                                <p>1987</p>
                            </div>
                            <div class="ml-4 text-right">
                                <p>東帝士集團 總管理部資材處課長</p>
                                <p>研究開發部專員</p>
                                <p>營繕專員</p>
                            </div>
                        </div>
                        <div class="w-full flex items-start justify-between text-[#968E85]">
                            <div class="w-[70px] md:w-[110px] flex justify-between shrink-0">
                                <p>1983-</p>
                                <p>1987</p>
                            </div>
                            <p class="ml-4">淡江大學土木工程學系 學士</p>
                        </div>
                    </div>
                </div>
                <div class="w-full md:flex justify-end mt-10 text-base">
                    <div class="bubble  flex items-center justify-center"
                        :class="[clientWidth < 770 ? 'bubble-bottom' : 'bubble-right']">
                        <p class="text-sm">一棟住宅的結構安全取決於是否有完善並且公開透明的施工品質。</p>
                    </div>
                    <div>
                        <img class="w-[200px] h-[200px] ml-auto" src="@/assets/images/avatar_yeh.png" alt="">
                        <div class="w-[300px] ml-auto flex flex-col items-end px-5">
                            <p
                                class="bg-[#CABFB3] text-sm  tracking-[2.5px] mr-[-2.5px] rounded-sm text-[white] inline-block px-1.5">
                                凱元土木包工業</p>
                            <div class="mt-2 flex items-end gap-12">
                                <div class="">
                                    <p class="text-[#756C62] text-[13px] tracking-[5px]">技術顧問</p>
                                    <p class="mt-[-1px] text-[#968E85] text-xs  tracking-[1px]">TECHNICAL<br/>ADVISER</p>
                                </div>
                                <div class="text-right">
                                    <p class="text-[24px] text-[#3C3C3C]">葉瑞銘</p>
                                    <p class="text-[#979797] text-xs mt-1.5 tracking-[2.5px]">Jui-Ming Yeh</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
defineProps({
    clientWidth: [Number]
})
</script>

<style scoped>
.bubble {
    box-sizing: border-box;
    position: relative;
    width: 100%;
    background: #813b31;
    border-radius: 999px;
    color: #fff;
    height: 75px;
    padding: 20px;
    margin-top: 20px;
}

.bubble-left {
    background: #484848 !important;
}

.bubble-top {
    background: #484848 !important;
}

.bubble-top:after {
    content: '';
    position: absolute;
    width: 0;
    height: 0;
    top: -40px;
    right: 240px;
    border-top: 20px solid transparent;
    border-bottom: 30px solid #484848;
    border-right: 20px solid transparent;
    border-left: 20px solid transparent;
}

.bubble-left:after {
    content: '';
    position: absolute;
    width: 0;
    height: 0;
    top: 20px;
    left: -40px;
    border-top: 20px solid transparent;
    border-bottom: 20px solid transparent;
    border-left: 20px solid transparent;
    border-right: 30px solid #484848;
}

.bubble-right:after {
    content: '';
    position: absolute;
    width: 0;
    height: 0;
    top: 30px;
    right: -40px;
    border-radius: 10px;
    border-top: 10px solid transparent;
    border-bottom: 20px solid transparent;
    border-right: 20px solid transparent;
    border-left: 30px solid #813b31;
}

.bubble-bottom:after {
    content: '';
    position: absolute;
    width: 0;
    height: 0;
    bottom: -40px;
    right: 130px;
    border-bottom: 20px solid transparent;
    border-top: 30px solid #813b31;
    border-right: 20px solid transparent;
    border-left: 20px solid transparent;
}
</style>