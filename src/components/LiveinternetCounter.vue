<template>
    <!--LiveInternet counter-->
        <a 
            href="//www.liveinternet.ru/click"
            target="_blank"
        >
                <img ref="licnt6B07" :width="width" :height="height" style="border:0" 
                    title="LiveInternet: показано число просмотров за 24 часа, посетителей за 24 часа и за сегодня"
                    src="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAEALAAAAAABAAEAAAIBTAA7"
                    alt=""
                />
        </a>
    <!--/LiveInternet-->
</template>

<script>
export default {
    components: {
    },
    props: {
        width: {
            type: Number, 
            default: 88
        }, 
        height:{
            type: Number, 
            default: 31
        },
        type: {
            type: Number, 
            default: 14
        }, 
        color:{
            type: Number, 
            default: 11
        }
    },

    data() {
        return {
        }
    },

    mounted() {
        const d = document;
        const s = screen;
        this.$refs.licnt6B07.src = "//counter.yadro.ru/hit?t" + this.type + "." + this.color +
            ";r"+escape(d.referrer)+
            ((typeof(s)=="undefined")?"":";s"+s.width+"*"+s.height+"*"+
                (s.colorDepth?s.colorDepth:s.pixelDepth))+";u"+escape(d.URL)+
                ";h"+escape(d.title.substring(0,150))+";"+Math.random()
    }

}
</script>


<style scoped>

        
</style>
