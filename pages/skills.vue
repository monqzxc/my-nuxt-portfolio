<script setup>
	import { TresCanvas } from "@tresjs/core";
	const { onLoop } = useRenderLoop();
	const boxRef = shallowRef(null);
	onLoop(({ delta, elapsed }) => {
		// I will run at every frame ~ 60FPS (depending of your monitor)
		if (boxRef.value) {
			boxRef.value.rotation.y += delta;
			boxRef.value.rotation.z = elapsed * 0.2;
		}
	});
</script>
<template>
	<TresCanvas>
		<TresMesh ref="boxRef" :scale="1">
			<TresBoxGeometry :args="[1, 1, 1]" />
			<TresMeshNormalMaterial />
		</TresMesh>
	</TresCanvas>
</template>
