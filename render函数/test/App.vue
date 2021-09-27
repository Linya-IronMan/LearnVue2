
<script>
import test1 from "./test1.vue"
import test2 from "./test2.vue"
export default {
    name: "APP",
    components: {
        test1,
        test2
    },
    render(h) {

        return h(
            "div",
            null,
            [
                h("test1"),
                h("test2")
            ]
        )
    }
}
</script>

<style>

</style>