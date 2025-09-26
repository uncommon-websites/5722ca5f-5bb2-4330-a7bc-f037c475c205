<script lang="ts">
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";

	type Props = {
		title: string;
		subtitle: string;
		imageSrc?: string;
		[key: string]: any;
	};

	let {
		title,
		subtitle,
		imageSrc = "https://www.unc.mn/image-placeholder.svg",
		...rest
	}: Props = $props();
</script>

<header class={[
	"border-b border-gray-100 dark:border-gray-900",
	"bg-gradient-to-br from-gray-900 via-gray-800 to-gray-900",
	"text-white"
]} {...rest}>
	<div class="section-px section-py container mx-auto grid gap-16 gap-y-0 max-w-6xl">
		<SectionHeader {title} {subtitle} size="lg" class="text-white" />
		<div class="aspect-video overflow-clip rounded-xl bg-gray-800 border border-gray-700">
			<img
				class="h-full w-full object-cover opacity-90 hover:opacity-100 transition-opacity duration-300"
				src={imageSrc}
				alt="SuccessVariable team collaborating on modern software solutions"
			/>
		</div>
	</div>
</header>
