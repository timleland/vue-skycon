<template>
<canvas :id="id" :width="width" :height="height"></canvas>
</template>

<script>
import Skycons from './skycons';

export default {
    props: {
        width: {
            type: [String, Number],
            default: 64
        },
        height: {
            type: [String, Number],
            default: 64
        },
        condition: {
            type: String
        },
        color: {
            type: String,
            default: 'black'
        }
    },
    data: function () {
        return {
            id: 'canvas' + Date.now().valueOf() + Math.floor(10000 * Math.random()),
            skycons: null
        };
    },
    created() {
        this.create();
    },
    methods: {
        create() {
            // initialize skycons
            this.destroy();
            this.skycons = new Skycons({
                color: this.color
            });
            this.skycons.play();
        },
        destroy() {
            if (this.id && this.skycons) {
                this.skycons.remove(this.id);
            }
        }
    },
    watch: {
        condition(value) {
            value = value.toUpperCase().replace(/-/g, '_');
            if (this.skycons) {
                this.skycons.set(this.id, Skycons[value]);
            }
        },
        options(value) {
            this.create(value);
        }
    },
    destroyed() {
        this.destroy();
    }
};
</script>
