<script>
	import '../app.css';
</script>

<nav class="mb-4 flex justify-between bg-blue-600 px-4 py-2 text-xl text-white sm:h-24">
	<div class="container mx-auto sm:flex sm:justify-between">
		<div class="flex items-center justify-between space-x-2">
			<a href="/" class="mr-0 text-2xl font-extrabold text-green-400 sm:mr-6">DM</a>
			<span class="font-bold sm:hidden">Devon McClure</span>
			<a class="hidden rounded px-2 py-1 hover:bg-red-500 sm:block" href="/">Home</a>
			<!-- <a class="hidden rounded px-2 py-1 hover:bg-red-500 sm:block" href="/projects">Projects</a>
			<a class="hidden rounded px-2 py-1 hover:bg-red-500 sm:block" href="/musings">Musings</a> -->
			<button type="button" class="hover:text-red-500 sm:hidden">
				<svg
					xmlns="http://www.w3.org/2000/svg"
					fill="none"
					viewBox="0 0 24 24"
					stroke-width="1.5"
					stroke="currentColor"
					class="h-8 w-8 cursor-pointer fill-current"
				>
					<path
						stroke-linecap="round"
						stroke-linejoin="round"
						d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
					/>
				</svg>
			</button>
		</div>

		<div class="py-2 sm:flex sm:items-center sm:justify-between">
			<div class="flex flex-col text-center sm:ml-6 sm:flex-row">
				<a class="rounded px-2 py-1 hover:bg-red-500 sm:hidden" href="/">Home</a>
				<!-- <a class="rounded px-2 py-1 hover:bg-red-500 sm:hidden" href="/projects">Projects</a>
				<a class="rounded px-2 py-1 hover:bg-red-500 sm:hidden" href="/musings">Musings</a> -->
				<hr class="my-4 border-white sm:hidden" />
				<a class="rounded px-2 py-1 hover:bg-red-500" href="mailto:contact@devonmcclure.dev">Email</a>
				<a class="rounded px-2 py-1 hover:bg-red-500" href="https://github.com/devonrmcclure">GitHub</a>
				<a class="rounded px-2 py-1 hover:bg-red-500" href="https://www.linkedin.com/in/devon-r-mcclure"LinkedIn</a>
			</div>
		</div>
	</div>
</nav>

<main class="container mx-auto p-4 leading-loose sm:p-0">
	<slot />
</main>

<footer class="container mx-auto flex justify-center p-4 text-green-500 sm:px-0">Devon McClure &copy; 2023</footer>

<style lang="postcss">
	:global(html) {
		background-color: theme(colors.slate.900);
		color: white;
	}
</style>
