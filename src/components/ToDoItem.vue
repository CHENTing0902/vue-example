<template>
    <div>
        <input type="checkbox" id="todo-item" :checked="done" />
        <label for="todo-item">{{label}}</label>
    </div>
</template>

<script>
export default {
    props: {
        label: { require: true, type: String },
        done: { default: false, type: Boolean},
        id: { require: true, tyep: String }
    },
    data() {
        return {
            idDone: this.done
        }
    }
};
</script>
