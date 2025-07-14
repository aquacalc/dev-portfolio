<script lang="ts">
	import { goto } from '$app/navigation';
	import { Button, SectionHeadline } from '$lib';

	// const onclick = () => goto('/#contact-form');
	function onclick() {
		goto('/#contact-form');
	}
</script>

<!-- <SectionHeadline sectionName='Gazda'>Gazda vode</SectionHeadline> -->

<section class="hero-section default-margin">
  <h3>Welcome!</h3>
  <div class="underscore mb-m"></div>

	<!-- <h2 class="dark-grey">Aquaculture</h2> -->
	<h2 class="dark-grey">Water chemistry</h2>
	<h2 class="dark-grey">as intuitive as</h2>
	<h2 class="mb-m">Google Maps</h2>

	<Button {onclick}>Let's get in contact!</Button>
</section>

<style>
	.hero-section {
		padding-top: min(3.5rem, 6%);
	}
</style>
