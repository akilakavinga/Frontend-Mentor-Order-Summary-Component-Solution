<section class="plan-tile">
    <img src="icon-music.svg" alt="music note icon" />
    <div class="plan-price-container">
        <h3 class="plan">Annual Plan</h3>
        <span class="price">$59.99/year</span>
    </div>
    <a href="/" class="change">Change</a>
</section>

<style lang="scss">
    @use "$lib/styles" as *;

    .plan-tile {
        @include flexRow;
        background: $veryPaleBlue;
        padding: 1.125rem 1.125rem;
        border-radius: 1rem;
        width: 100%;

        .plan-price-container {
            line-height: 1.4rem;
            margin-inline: 1.25rem 3rem;
            .plan {
                font-size: 0.94rem;
                color: $darkBlue;
                font-weight: 900;
                width: max-content;
            }

            .price {
                color: $desaturatedBlue;
                font-size: 0.96rem;
            }
        }
        .change {
            color: $brightBlue;
            font-weight: 900;
            font-size: 0.85rem;
            transition: opacity 75ms ease;

            &:hover {
                opacity: 0.6;
            }
        }
    }
</style>
