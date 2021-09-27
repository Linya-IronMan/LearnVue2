
<script>
export default {
    render(createElement) {
        const vnode = createElement(
            "div",
            {
                class:"xxclas",
                // style
                style: {
                    color: "red",
                },
                // 设置 html 内容
                // domProps: { innerHTML: "helloworld" },
                // 设置 html 属性
                attrs: {
                    id: "#app"
                }
            },
            [ createElement('h1', null,  "没有什么能够阻挡"),createElement('h1', null,  "傻妞 开机") ]
        )
        console.log(vnode, "======")
        return vnode;
    }
}
</script>

<style>

</style>