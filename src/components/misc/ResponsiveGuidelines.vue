<template>
    <div>
        <div id="xs" class="tick-container">
            <span class="tick-label">
                xs
                <br />600
            </span>
        </div>
        <div id="guideline-xs" class="guideline"></div>

        <div id="sm" class="tick-container">
            <span class="tick-label">
                sm
                <br />960
            </span>
        </div>
        <div id="guideline-sm" class="guideline"></div>
        <div id="md" class="tick-container">
            <span class="tick-label">
                md
                <br />1264
            </span>
        </div>
        <div id="guideline-md" class="guideline"></div>

        <div id="lg" class="tick-container">
            <span class="tick-label">
                lg
                <br />1904
            </span>
        </div>
        <div id="guideline-lg" class="guideline"></div>
    </div>
</template>

<script lang="ts">
export default {};
</script>

<style lang="scss">
@use"../../main";

.tick-container {
    position: fixed;
    box-sizing: content-box;
    height: 20px;
    display: inline-block;
    border-right: 1px solid main.$gray-light;
    z-index: 1000;
}

.tick-label {
    font-size: 8px;
    text-align: right;
    color: main.$gray-light;
}

.guideline {
    position: fixed;
    top: 0;
    height: 100vh;
    border-right: 1px dashed main.$gray-light;
    opacity: 0.5;
    box-sizing: content-box;
    z-index: 1001;
}

#xs,
#sm,
#md,
#lg {
    padding-right: 3px;
    position: fixed;
    z-index: 1000;
    position: fixed;
    top: 2px;
    font-size: 8px;
    text-align: right;
    color: main.$gray-light;
}

#xs {
    left: 583px;
}
#sm {
    left: 943px;
}
#md {
    left: 1242px;
}
#lg {
    left: 1882px;
}

#guideline-xs {
    left: 599px;
}
#guideline-sm {
    left: 959px;
}
#guideline-md {
    left: 1263px;
}
#guideline-lg {
    left: 1903px;
}
</style>
