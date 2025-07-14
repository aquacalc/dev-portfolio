<script lang="ts">
	import { goto } from '$app/navigation';
	import { SectionHeadline, Button } from '$lib';

  function onclick() {
    goto('/#contact-form')
  }
</script>

<section class="about-me mt-l">
	<SectionHeadline sectionName={'about-me'}>
		<h2>About Me</h2>
	</SectionHeadline>
	<div class="content-container default-margin mt-m">
		<img class="image" src="about-me.jpeg" alt="about me photo" />
		<div class="text">
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugit ut corporis inventore hic,
				quam saepe, recusandae illum, ab voluptatem quas ullam cumque eveniet. Non excepturi quia
				inventore eos totam, molestiae molestias culpa fugit dolorem. Sint unde iure magnam, modi
				saepe minus facere maxime possimus odit, non fugiat omnis, vel itaque.
			</p>

			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugit ut corporis inventore hic,
				quam saepe, recusandae illum, ab voluptatem quas ullam cumque eveniet. Non excepturi quia
				inventore eos totam, non fugiat omnis, vel itaque.
			</p>

			<!-- <p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugit ut corporis inventore hic,
				quam saepe, recusandae illum, ab voluptatem quas ullam cumque eveniet. Non excepturi quia
				inventore eos totam, molestiae molestias culpa fugit dolorem. Sint unde iure magnam, modi
				saepe minus facere maxime possimus odit, non fugiat omnis, vel itaque.
			</p> -->
      <Button className='mt-m' {onclick}>Tell me about your project</Button>
		</div>
	</div>
</section>

<style>
	.content-container {
		display: flex;
		justify-content: space-between;
    align-self: stretch;
	}

	.image {
		width: 42%;
    border-radius: 20px;
    object-fit: cover;
	}

  .text {
    width: 55%;
    text-align: left;
  }
</style>
