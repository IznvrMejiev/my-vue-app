<template>
    <div class="videos">
        <div class="video" @click="videos[0] = !videos[0]"> 
            <div class="nomer">01</div>
            <div class="info">
                <h4>Упражнения дома</h4>
                <p>15 видео</p>
            </div>
            <div class="icon"><i class="fa-solid fa-arrow-right"></i></div>
             <div class="video__open" v-if="videos[0]">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ullam magni sequi officiis itaque illum blanditiis ab doloremque, tempora consequatur eligendi eaque vero obcaecati, et consectetur vel molestias dolore ut. Fuga.
             </div>
        </div>
        <div class="video" @click="videos[1] = !videos[1]">
            <div class="nomer">02</div>
            <div class="info">
                    <h4>Упражнения дома</h4>
                <p>15 видео</p>
            </div>
            <div class="icon"><i class="fa-solid fa-arrow-right"></i></div>
               <div class="video__open" v-if="videos[1]">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ullam magni sequi officiis itaque illum blanditiis ab doloremque, tempora consequatur eligendi eaque vero obcaecati, et consectetur vel molestias dolore ut. Fuga.
             </div>
        </div>
        <div class="video" @click="videos[2] = !videos[2]">
            <div class="nomer">03</div>
            <div class="info">
                    <h4>Упражнения дома</h4>
                <p>15 видео</p>
            </div>
            <div class="icon"><i class="fa-solid fa-arrow-right"></i></div>
               <div class="video__open" v-if="videos[2]">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ullam magni sequi officiis itaque illum blanditiis ab doloremque, tempora consequatur eligendi eaque vero obcaecati, et consectetur vel molestias dolore ut. Fuga.
             </div>
        </div>
        <div class="video" @click="videos[3] = !videos[3]">
            <div class="nomer">04</div>
            <div class="info">
                    <h4>Упражнения дома</h4>
                <p>15 видео</p>
            </div>
            <div class="icon"><i class="fa-solid fa-arrow-right"></i></div>
               <div class="video__open" v-if="videos[3]">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ullam magni sequi officiis itaque illum blanditiis ab doloremque, tempora consequatur eligendi eaque vero obcaecati, et consectetur vel molestias dolore ut. Fuga.
             </div>
        </div>
        <div class="video" @click="videos[4] = !videos[4]">
            <div class="nomer">05</div>
            <div class="info">
                    <h4>Упражнения дома</h4>
                <p>15 видео</p>
            </div>
            <div class="icon"><i class="fa-solid fa-arrow-right"></i></div>
               <div class="video__open" v-if="videos[4]">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ullam magni sequi officiis itaque illum blanditiis ab doloremque, tempora consequatur eligendi eaque vero obcaecati, et consectetur vel molestias dolore ut. Fuga.
             </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return{
            videos: [false, false, false, false, false]
        }
    }
};


</script>


<style scoped lang="scss">

.videos {
    margin-top: 250px;
}

.video {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 40px 0px;
    cursor: pointer;
    transition: all 500ms ease;
    flex-wrap: wrap;



    &:not(:last-of-type) {
        border-bottom: 0.5px solid #666666;
    }

    &:hover {
        background: #1d1d1d;

        i {
            transform: rotate(90deg);
        }
    }

    .video__open {
        width: 100%;
        margin: 30px 50px;
        margin-bottom: 10px;
    }

    .nomer {
        color: #575757;
        font-weight: 600;
        font-size: 1.2em;
        
    }

    .info {
          @media(min-width: 630px) {
        
          width: 450px;

        }
        @media(max-width: 630px) {
        
                  width: 200px;
        }
    }

    h4 {
        font-weight: 400;
        @media(min-width: 630px) {
        
            font-size: 2.5em;

        }
        @media(max-width: 630px) {
        
            font-size: 1.5em;

        }
    }

    p {
        color: #6f6f6f;
        margin-top: 10px;
    }

    i {
        margin-right: 20px;
        transition: all 500ms ease;
    }

}


</style>