<template>
    <div class="list">
        <div class="list__avatar">
            <img src="@assets/images/user-01.png" alt="" class="list__avatar__image" />
            <div class="list__avatar__text-box">
                <span class="name">Marco</span>
                <span class="duty">User Experience</span>
            </div>
        </div>
        <div class="list__resume-score"></div>
        <div class="list__skill-match"></div>
        <div class="list__rank">
            <!-- <div class="chip">Senior</div> -->
        </div>
    </div>
</template>

<script setup lang="ts"></script>

<style lang="scss" scoped>
.list {
    display: flex;
    align-items: center;

    width: calc(100% - 32px);
    height: 72px;
    min-height: 72px;

    padding: 0 16px;

    background-color: rgba($color-white-200, 0.1);
    border-radius: 16px;

    &__avatar {
        display: flex;
        align-items: center;
        justify-content: center;

        gap: 8px;

        &__image {
            width: 44px;
            height: 44px;

            border-radius: 50%;
            border: 1px solid rgba($color-white-200, 0.3);
        }
        &__text-box {
            display: flex;
            flex-direction: column;

            gap: 4px;

            .name {
                color: $color-black-900;
            }
            .duty {
                font-size: 14px;
                font-weight: 300;
                color: $color-white-200;
            }
        }
    }
}
</style>
