<script lang="ts">
	import { goto } from '$app/navigation';
	import Button from './Button.svelte';

	// const onclick = () => goto('/#contact-form');
	function onclick() {
		goto('/#contact-form');
	}
</script>

<section class="hero-section default-margin">
	<h3>Gazda vode</h3>
	<div class="underscore mb-m"></div>

	<h2 class="dark-grey">Water chemistry</h2>
	<h2 class="dark-grey">as intuitive as</h2>
	<h2 class='mb-m'>as Google Maps</h2>

	<Button {onclick}>Let's get in contact!</Button>
</section>

<style>
	.hero-section {
		padding-top: min(3.5rem, 6%);
	}
</style>
