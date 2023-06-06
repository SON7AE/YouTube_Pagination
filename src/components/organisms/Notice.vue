<template>
    <div class="notice">
        <div class="notice__header">
            <div class="notice__header__total">
                <span class="count">142</span>
                <span class="label">Candidates</span>
            </div>
            <div class="notice__header__info">
                <div class="item">
                    <span class="item__top">All</span>
                    <span class="item__bottom">Best In</span>
                </div>
                <div class="item">
                    <span class="item__top">All</span>
                    <span class="item__bottom">Best In</span>
                </div>
                <div class="item">
                    <span class="item__top">Default</span>
                    <span class="item__bottom">Sort Results</span>
                </div>
            </div>
        </div>
        <div class="notice__body">
            <div class="notice__body__column"></div>
            <div class="notice__body__list-box">
                <div class="list">
                    <div class="list__avatar">
                        <img src="" alt="" />
                        <div class="list__avatar__text-box">
                            <span class="name"></span>
                            <span class="duty"></span>
                        </div>
                    </div>
                    <div class="list__resume-score"></div>
                    <div class="list__skill-match"></div>
                    <div class="list__rank">
                        <div class="chip">Senior</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts"></script>

<style lang="scss" scoped>
.notice {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    width: calc(100% - 36px);
    height: 100%;

    padding: 0 12px 0 24px;

    &__header {
        display: flex;
        align-items: center;
        justify-content: space-between;

        width: 100%;

        padding-bottom: 12px;

        border-bottom: 1px solid $color-white-200;

        &__total {
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            justify-content: center;

            .count {
                font-family: 'MBC1961GulimM';
                font-size: 18px;
            }
            .label {
                font-family: 'SUITE-Regular';
                color: $color-white-200;
            }
        }
        &__info {
            display: flex;
            align-items: center;

            gap: 40px;

            .item {
                display: flex;
                flex-direction: column;
                align-items: flex-start;
                justify-content: center;

                &__top {
                    font-family: 'MBC1961GulimM';
                    color: $color-blue-000;
                }
                &__bottom {
                    font-family: 'SUITE-Regular';
                    color: $color-white-200;
                }
            }
        }
    }
    &__body {
    }
}
</style>
