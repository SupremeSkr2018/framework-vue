<template>
	<div>
		<div class="hello">hello,{{ age }}</div>
		<el-button type="primary">主要按钮</el-button>
	</div>
</template>
<script lang="ts">
import Vue from 'vue';
import Component from 'vue-class-component';
@Component({
	name: 'Hello'
})
export default class Hello extends Vue {
	private age: number = 12;
	mounted() {
		console.log('Hello Component mounted', this.age);
	}
}
</script>
<style lang="less" scoped module>
.hello {
	background: lightblue;
}
.wrap {
	border: 1px solid red;
	background: lightseagreen;
}
</style>
