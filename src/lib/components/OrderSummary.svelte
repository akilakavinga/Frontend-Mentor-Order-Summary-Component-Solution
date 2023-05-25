<script>
    import PlanTile from "./PlanTile.svelte";
</script>

<section class="order-summary">
    <img src="illustration-hero.svg" alt="" />
    <div class="bottom">
        <h1>Order Summary</h1>
        <p>
            You can now listen to millions of songs, audiobooks, and podcasts on
            any device anywhere you like!
        </p>
        <PlanTile />
        <button class="proceed">Proceed to Payment</button>
        <button class="cancel">Cancel Order</button>
    </div>
</section>

<style lang="scss">
    @use "$lib/styles" as *;

    .order-summary {
        @include flexCol;
        justify-content: space-between;
        max-width: 375px;
        border-radius: 1.5rem;
        overflow: hidden;
        background-color: white;
        box-shadow: 0 10px 10px rgba($desaturatedBlue, 0.2);
        @include mqPhone {
            max-width: 340px;
        }

        img {
            width: 100%;
        }

        .bottom {
            @include flexCol;
            max-width: 300px;
            justify-content: space-evenly;
            margin: 2rem 0 1.9rem;

            h1 {
                font-size: 1.4rem;
                font-weight: 900;
                color: $darkBlue;
            }

            p {
                color: $desaturatedBlue;
                text-align: center;
                max-width: 18rem;
                line-height: 1.5rem;
                font-size: 0.95rem;
                margin: 1rem 0 1.5rem;
                @include mqPhone {
                    max-width: 16rem;
                }
            }

            .proceed {
                width: 100%;
                background-color: $brightBlue;
                border: none;
                color: white;
                font-weight: 700;
                font-size: 1rem;
                padding: 1rem;
                border-radius: 0.8rem;
                box-shadow: 0 20px 15px rgba($brightBlue, 0.18);
                margin: 1.75rem 0 1.5rem;
                cursor: pointer;
                transition: opacity 75ms ease;

                &:hover {
                    opacity: 0.6;
                }
            }

            .cancel {
                background-color: transparent;
                border: none;
                color: $desaturatedBlue;
                font-weight: 900;
                font-size: 0.94rem;
                cursor: pointer;
                transition: color 75ms ease;

                &:hover {
                    color: $darkBlue;
                }
            }
        }
    }
</style>
