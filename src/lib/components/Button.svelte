<script lang="ts">
	import type { Snippet } from 'svelte';

	interface ButtonProps {
		children: Snippet;
		onclick: (e: MouseEvent) => void | (() => void);
		className?: string;
	}

	let { children, className, ...props }: ButtonProps = $props();
</script>

<button class={`btn ${className}`} {...props}>{@render children()}</button>

<style>
  .btn {
    font-family: 'Inter Tight', sans-serif;
    font-weight: 500;
    background-color: blue;
    color: white;
    font-size: 24px;
    padding: 14px 40px;
    border-radius: 10px;
  }
	/* button {
		background-color: rgb(0, 58, 128);
		color: white;
		padding: 20px 24px;
		font-weight: normal;
		font-size: 22px;
		text-transform: uppercase;
		transition: all 500ms;
		border: 1px solid rgb(0, 58, 128);
		border-radius: 8px;
	} */

	button:hover {
		background-color: rgba(0, 58, 128, 0.7);
		/* color: black; */
	}
</style>
