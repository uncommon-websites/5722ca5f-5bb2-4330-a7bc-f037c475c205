<script lang="ts">
	// Components
	import AnimateText from "$lib/components/animation/AnimateText.svelte";

	type Props = {
		title: string;
		subtitle: string;
		oncomplete?: () => void;
		size?: "sm" | "lg";
		class?: string;
	};

	let {
		title = "",
		subtitle = "",
		oncomplete = () => {},
		size = "sm",
		class: className = ""
	}: Props = $props();
</script>

<div
	class={[
		"section-pb-sm container-sm grid text-balance",
		size === "lg" ? "text-display" : "text-title2",
		className
	]}
>
	<h2>
		<AnimateText text={title} {oncomplete} />
	</h2>
	<p class={[
		"text-emphasis-dim",
		className.includes("text-white") ? "text-gray-300" : ""
	]}>
		<AnimateText text={subtitle} />
	</p>
</div>
