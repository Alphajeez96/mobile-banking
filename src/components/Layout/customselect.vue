<template>
  <div class="custom-select" :tabindex="tabindex" @blur="open = false">
    <div class="selected" :class="{open: open}" @click="open = !open">{{ selected }}</div>
    <div class="items" :class="{selectHide: !open}">
      <div
        class="item"
        v-for="(option, i) of options"
        :key="i"
        @click="selected=option; open=false; $emit('input', option)"
      >{{ option }}</div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    options: {
      type: Array,
      required: true
    },
    tabindex: {
      type: Number,
      required: false,
      default: 0
    }
  },
  data() {
    return {
      selected: this.options.length > 0 ? this.options[0] : null,
      open: false
    };
  },
  mounted() {
    this.$emit("input", this.selected);
  }
};
</script>

<style scoped>
.custom-select{
    background: #FFFFFF;
border: 0.5px solid #F2F2F2;
box-sizing: border-box;
box-shadow: 0px 5px 20px rgba(0, 0, 0, 0.08);
}


.selected {
 

font-size: 12px;
border-radius: 5px;
  color: black;
    padding: 4px 10px;
  cursor: pointer;
  user-select: none;
}

.selected.open {
border: 1px solid #A9A5AF;
  border-radius: 6px 6px 0px 0px;
}

.selected:after {
  position: absolute;
  content: "";
  top: 22px;
  right: 10px;
  width: 0;
  height: 0;
  border: 4px solid transparent;
  border-color: #fff transparent transparent transparent;
}

.items {
color: #03293D;
  border-radius: 0px 0px 6px 6px;
  overflow: hidden;
  /*border-right: 1px solid #CE9B2C;
  border-left: 1px solid #CE9B2C;
  border-bottom: 1px solid #CE9B2C;*/
  position: absolute;
  background: white;

  left: 0;
  right: 0;
}

.item {
color: #03293D;
font-size: 12px;
font-weight: bold;
text-align: center;
padding: 10px;
  cursor: pointer;
  user-select: none;
}

.item:hover {
background: #E8E7EA;
}

.selectHide {
  display: none;
}
</style>