<template>
  <div class="m-socialLinks">
        <h5>Follow Us</h5>
        <ul>
            <li>
                <a href="#">
                    <img src="../../assets/img/footer-facebook.png" alt="">
                </a>
                <a href="#">
                    <img src="../../assets/img/footer-twitter.png" alt="">
                </a>
                <a href="#">
                    <img src="../../assets/img/footer-youtube.png" alt="">
                </a>
                <a href="#">
                    <img src="../../assets/img/footer-pinterest.png" alt="">
                </a>
                <a href="#">
                    <img src="../../assets/img/footer-periscope.png" alt="">
                </a>
            </li>
        </ul>
  </div>
</template>

<script>
export default {

}
</script>

<style lang = "scss" scoped>
    .m-socialLinks{
        display: flex;
        align-items: center;
        column-gap: var(--space-md);
    }

    h5{
        text-transform: uppercase;
        color: var(--clr-primary);
        font-size: var(--fs-xl);
    }
    ul{
        list-style: none;
    }
    a{
        padding-right: var(--space-md);
    }
</style>