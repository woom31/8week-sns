<template>
    <div class="feed">
        <div class="feed-top">
            <img class="top-img" :src="item.image" alt="Profile image">
            <div class="top-profile">
                <div class="top-name">{{item.name}}</div>
                <div class="top-time">{{item.time}}</div>
            </div>
        </div>
        <div class="feed-body">
            <div class="body-content">{{item.content}}</div>
            <img class="body-image" :src="item.conimage" alt="Contents image">
        </div>
        <div class="feed-bottom">
            <a class="btn btn-like" @click="feedLike">
                <span class="material-icons icons">
                    favorite_border
                </span>
            </a>
            <a class="btn btn-comment" @click="feedComment">
                <span class="material-icons icons">
                    chat_bubble_outline
                </span>
            </a>
            <a class="btn btn-share" @click="feedShare">
                <span class="material-icons icons">
                    share
                </span>
            </a>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Feed',
    props: {
        item: Object
    },
    methods : {
        feedLike(){
            console.log('Like!')
            
        },
        feedComment(){
            console.log('Comment!')
        },
        feedShare(){
            console.log('Share!')
        }
    }
}
</script>

<style scoped>


</style>