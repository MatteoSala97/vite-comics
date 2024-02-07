<script>

export default {
  name: "JumbotronApp"
}
</script>

<template>
    <div class="jumbo">
        <p>
            -- Content goes here --
        </p>
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

    div{
        background-color: #1c1c1c;
        text-align: start;
        padding: 100px;

        p{
            font-size: 30px;
            color: white;
        }
    }

</style>