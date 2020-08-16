<template>
    <div>
    <!-- side nav here -->
    <aside class="side__nav">
        <span class="side__logo px-3 py-4">
<img src="../../assets/General/sidelogo.png" alt="">
        </span>
        <div class="border-b"></div>
    </aside>
    </div>
</template>

<style scoped>
    .side__nav {
        position: fixed;
        height: 100%;
        background: #052231;
        overflow: auto;
        width: 80px;
    }
    
    .side__logo {
        display: flex;
        width: 100%;
        align-items: center;
    }
    
    .border-b {
        border-bottom: 1px solid #E8E7EA;
        opacity: 0.1;
    }
</style>