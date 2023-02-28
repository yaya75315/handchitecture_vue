<template>
    <div class="custom-cursor">
        <div id="cursor-big" class="custom-cursor__ball custom-cursor__ball--big"></div>
    </div>
</template>
  
<script>
import gsap from "gsap";

export default {
    mounted() {
        const cursorBig = document.getElementById('cursor-big'),
            links = document.getElementsByTagName("li"),
            icons = document.getElementsByTagName("a"),
            buttons = document.getElementsByTagName("button"),
            withHover = [...links, ...buttons, ...icons];

        // Event Listeners
        document.addEventListener("mousemove", onMouseMove);
        document.addEventListener("mousedown", onMouseHover);
        document.addEventListener("mouseup", onMouseHoverOut);
        document.addEventListener("mouseenter", () => {
            cursorBig.style.opacity = 1;
        });
        document.addEventListener("mouseleave", () => {
            cursorBig.style.opacity = 0;
        });
        withHover.forEach((element) => {
            element.addEventListener("mouseover", onMouseHover);
            element.addEventListener("mouseout", onMouseHoverOut);
        })

        // Event Handlers
        function onMouseMove(e) {
            gsap.to(cursorBig, {
                x: e.clientX - 18,
                y: e.clientY - 18,
                direction: 0.4
            });
        }
        function onMouseHover() {
            gsap.to(cursorBig, {
                scale: 3,
                direction: 0.3
            });
        }
        function onMouseHoverOut() {
            gsap.to(cursorBig, {
                scale: 1,
                direction: 0.3
            });
        }
    }
};
</script>
  
<style scoped>
.custom-cursor__ball {
    position: fixed;
    top: 0;
    left: 0;
    z-index: 99999;
    background: #e5e7eb5A;
    pointer-events: none;
    transition: opacity 0.5s ease;
}

.custom-cursor__ball--big {
    content: "";
    width: 35px;
    height: 35px;
    background: #D9D9D95A;
    border-radius: 50%;
}
</style>
  