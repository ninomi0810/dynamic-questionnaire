<script>
import check from '../views/frontChack.vue'
import FeedbackDetail from '../views/FeedbackDetail.vue'
export default {
    data() {
        return {
            name: "",
            tel: "",
            email: "",
            age: "",
        }
    },
    components: {
        check
    }
}
</script>
<template>
    <div class="time">
        <p>問卷填寫時間</p>
    </div>
    <div class="title">
        <p>問卷名稱</p>
    </div>
    <div class="produce">
        <p>問卷介紹</p>
    </div>
    <div class="content">
        <div class="information">
            <div class="one">
                <span>姓名：</span>
                <input type="text" name="" id="" v-model="this.name">
            </div>
            <div class="two">
                <span>手機：</span>
                <input type="tel" name="" id="" v-model="this.tel">
            </div>
            <div class="three">
                <span>E-mail：</span>
                <input type="emil" name="" id="" v-model="this.email">
            </div>
            <div class="four">
                <span>年齡：</span>
                <input type="number" name="" id="" v-model="this.age">
            </div>
        </div>
        <div class="question">
            <div class="one"></div>
            <div class="two"></div>
            <div class="three"></div>
        </div>
    </div>
    <div class="footer">
        <button type="submit" class="rounterItem">
            <RouterLink :to="`/Front`">取消</RouterLink>
        </button>
        <button type="submit" class="rounterItem">
            <RouterLink :to="`/FrontChack`">送出</RouterLink>
        </button>
    </div>
</template>

<style scoped lang="scss">
.time {
    width: 30vw;
    height: 7vh;
    margin-left: 40%;
    margin-top: 3%;
    font-size: 16px;
    border: 1px solid black;
}

.title {
    width: 80vw;
    height: 10vh;
    font-size: 28px;
    border: 1px solid black
}

.produce {
    width: 80vw;
    height: 15vh;
    font-size: 28px;
    border: 1px solid black
}


.content {
    display: flex;
    justify-content: center;

    .information {
        width: 800px;
        height: 300px;
        border: 1px solid black;
        font-size: large;
        position: relative;

        span {
            width: 70px;
            position: absolute;
            left: 50px;
        }

        input {
            position: absolute;
            width: 500px;
            height: 25px;
            left: 200px;
        }

        .one {
            position: absolute;
            top: 20px;
        }

        .two {
            position: absolute;
            top: 80px;
        }

        .three {
            position: absolute;
            top: 140px;
        }

        .four {
            position: absolute;
            top: 200px;
        }
    }
}

.footer {
    .rounterItem {
        margin-left: 10px;
        text-decoration: none;
    }
}
</style>