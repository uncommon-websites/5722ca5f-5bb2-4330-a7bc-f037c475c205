<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Technical excellence",
			description: "Full-stack expertise across ERP, CRM, e-commerce, and logistics platforms built to enterprise standards."
		},
		{
			title: "Regulatory mastery",
			description: "Deep compliance knowledge for high-risk industries that others avoid, turning regulatory challenges into competitive advantages."
		},
		{
			title: "Growth acceleration",
			description: "Systems designed not just for compliance, but to unlock operational efficiency and new revenue streams at scale."
		}
	];
</script>

<SecondaryHero
	title="Move fast. Stay compliant."
	subtitle="Modern systems built for complex industries"
	imageSrc="/generated/image-a-group-of-diverse-professionals-engaged.webp"
/>

<!-- Story Section -->
<Story
	generating
	paragraphs={[
		"We started in 2018 with a simple goal: make helpful tech that people actually need. While many chase profits, we chose to do things differently.",
		"Beyond making good products, we care about doing the right thing, being kind to our planet, and making sure everyone can use what we build. That's our compass.",
		"From day one, we've asked ourselves: 'Does this actually help people?' This question gets us through tough calls and shapes who we are. We're playing the long game here.",
		"We think about how our work affects real people's lives. We build tech that brings people together, keeps your information safe, and treats everyone fairly. When we stick to these basics, good things happen."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Leadership."
	subtitle="Building the backbone for high-risk industries."
	stakeholders={[
		{
			name: "Oze Botach",
			position: "Founder & CEO",
			bio: "Combining deep regulatory expertise with rapid full-stack development to transform compliance challenges into growth opportunities for complex businesses.",
			image: "/generated/image-professional-executive-headshot-of-a-con.webp"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Stop losing time to regulators"
	subtitle="Start shipping faster"
	description="Join hundreds of executives using SuccessVariable to transform compliance headaches into growth opportunities. Get Fortune 100-grade systems built for your high-risk industry—from e-commerce platforms to ERP and logistics solutions that scale."
	imageSrc="/generated/image-a-group-of-executives-in-formal-business.webp"
/>
