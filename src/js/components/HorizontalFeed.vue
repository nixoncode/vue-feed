<template>
    <div class="horizontal-feed">
        <div class="header">
            <span v-text="header"></span>
        </div>
        <div class="body">
            <div>
                <p>
                    <a href="#">Title
                        <span>Content</span>
                    </a>
                </p>
            </div>
            <div class="cover"></div>
        </div>
        <div class="buttons">
            <span class="previous">
                <i class="fa fa-angle-left"></i>
            </span>
            <span class="play">
                <i class="fa fa-play"></i>
            </span>
            <span class="next">
                <i class="fa fa-angle-right"></i>
            </span>
        </div>
    </div>
</template>


<script>
export default {
    props: {
        duration: {
            type: Number,
            required: false,
            default: 7000,
        },
        header: {
            type: String,
            required: true,
        },
        collection: {
            type: [Array, String],
            required: true
        }
    }
}
</script>