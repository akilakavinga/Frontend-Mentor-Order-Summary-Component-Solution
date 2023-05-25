<section>
    <span>
        Challenge by
        <a href="https://www.frontendmentor.io/">Frontend Mentor</a>
    </span>
    <span>
        Coded by
        <a href="https://github.com/akilakavinga">Akila Kavinga</a>
    </span>
</section>

<style lang="scss">
    @use "$lib/styles" as *;
    section {
        @include flexCol;
        bottom: 5.5%;
        font-size: 0.8rem;
        line-height: 20px;
        background-color: $darkBlue;
        color: $desaturatedBlue;
        padding: 0.6rem 2.2rem;
        border-radius: 1rem;
        margin: 1rem 0 0;

        a {
            color: white;
            transition: opacity 75ms ease;

            &:hover {
                opacity: 0.6;
            }
        }
    }
</style>
