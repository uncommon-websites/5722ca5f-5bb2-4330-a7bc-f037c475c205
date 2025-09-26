<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CustomerCardHero from "$lib/components/layout/hero-sections/CustomerCardHero.svelte";
</script>

<CustomerCardHero
	centered={true}
	title="Turning compliance into competitive advantage"
	subtitle="High-risk and complex businesses trust SuccessVariable to build the modern software backbone that transforms regulatory challenges into scalable growth opportunities."
	customers={[
		{
			name: "Michael Chen",
			position: "CEO, SecureLogistics",
			imageSrc: "/generated/image-centered-portrait-of-a-professional-midd.webp"
		},
		{
			name: "Sarah Rodriguez",
			position: "CTO, ComplianceFirst",
			imageSrc: "/generated/image-centered-portrait-of-a-professional-woma.webp"
		},
		{
			name: "James Thompson",
			position: "Operations Director, FreightForward",
			imageSrc: "/generated/image-centered-portrait-of-a-mature-business-e.webp"
		},
		{
			name: "Elena Vasquez",
			position: "Chief Technology Officer, RiskVentures",
			imageSrc: "/generated/image-centered-portrait-of-a-professional-woma.webp"
		},
		{
			name: "Robert Kim",
			position: "Executive Vice President, CapitalBridge",
			imageSrc: "/generated/image-centered-portrait-of-a-senior-male-execu.webp"
		}
	]}
/>
<LogoScroller 
	label="Trusted by industry leaders"
	logoUrls={[
		'https://cdn.brandfetch.io/paypal.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/square.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/stripe.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/shopify.com/w/400/h/400/logo'
	]}
/>

<Summary
	generating
	title="What we do"
	text="Our technology delivers measurable results through secure, adaptable solutions that directly increase productivity and drive growth."
/>

<Testimonials
	testimonials={[
		{
			name: "Marcus Rivera",
			position: "CEO",
			company: "SecureFinance Solutions",
			quote:
				"SuccessVariable transformed our compliance nightmare into a competitive advantage. We went from 6-week payment processor approvals to same-day activations. Their regulatory expertise saved us $2.3M in potential fines and opened three new revenue channels we couldn't access before.",
			image: "/generated/image-professional-headshot-of-marcus-rivera-a.webp"
		},
		{
			name: "Diana Chen",
			position: "CTO",
			company: "RiskVault Technologies",
			quote:
				"Before SuccessVariable, we spent 40% of our engineering time on compliance patches. Now it's automated. Their full-stack platform reduced our operational overhead by 60% while eliminating the regulatory risks that kept me up at night. ROI was clear within 90 days.",
			image: "/generated/image-professional-headshot-of-diana-chen-an-a.webp"
		},
		{
			name: "Kevin O'Sullivan",
			position: "Operations Director",
			company: "CrossBorder Logistics",
			quote:
				"The regulatory complexity of international freight was strangling our growth. SuccessVariable built us a system that handles compliance across 15 countries automatically. We've cut processing time from 3 days to 4 hours and expanded into markets we never thought possible.",
			image: "/generated/image-professional-headshot-of-kevin-osullivan.webp"
		}
	]}
/>

<Features
	title="Built for high-risk, complex businesses"
	subtitle="We combine deep regulatory expertise with rapid full-stack development to turn compliance challenges into competitive advantages"
	features={[
		{
			title: "Regulatory compliance engine",
			description: "Automated compliance workflows keep you ahead of changing regulations while reducing legal risk by 85%.",
			imageSrc: "/generated/image-1-a-group-of-executives-in-formal-busine.webp"
		},
		{
			title: "High-risk payment processing",
			description: "Custom gateway solutions bypass processor rejections and unlock revenue streams traditional systems can't handle.",
			imageSrc: "/generated/image-2-employees-in-business-casual-clothing-.webp"
		},
		{
			title: "Full-stack business platforms",
			description: "Integrated ERP, CRM, and e-commerce systems built specifically for complex operational requirements.",
			imageSrc: "/generated/image-3-a-contemporary-open-office-space-with-.webp"
		},
		{
			title: "Automated compliance monitoring",
			description: "Real-time risk detection and proactive alerts prevent costly violations before they impact your business.",
			imageSrc: "/generated/image-4-a-spacious-organized-control-room-with.webp"
		},
		{
			title: "Legacy system modernization",
			description: "Seamless migration from outdated workflows to modern platforms without disrupting ongoing operations.",
			imageSrc: "/generated/image-5-a-split-scene-office-showing-one-side-.webp"
		},
		{
			title: "Strategic risk analytics",
			description: "Advanced data insights transform compliance costs into strategic advantages that drive measurable growth.",
			imageSrc: "/generated/image-6-a-lively-office-environment-where-a-di.webp"
		}
	]}
/>
<AboutTeaser generating />
<CallToAction generating />
