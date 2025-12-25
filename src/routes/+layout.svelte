<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
  import { goto } from '$app/navigation';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>
<!--Navbar-->

<div>
	<nav class="bg-gray-800 p-4 text-white">
		<div
			class="container mx-auto flex justify-between items-center"
		>
			<div>
				<a href="/" class="btn btn-ghost text-xl">EditIT</a>
				<a href="/user" class="btn btn-ghost">My page</a>
			</div>
			<div>
				<button onclick={()=>goto("/login")}>Login</button>
				<span class="text-white text-lg ml-2">hello1@gmail.com</span>
				<button onclick={()=>console.log("loging out")}>logout</button>
			</div>
		</div>
	</nav>
	
</div>

{@render children()}
