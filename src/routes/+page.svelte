<script>
	import { onMount } from 'svelte';

	let mounted = false;

	onMount(() => {
		mounted = true;
	});
</script>

<svelte:head>
	<title>Amethyst - Speedy Sites</title>
	<meta name="description" content="A beautiful, fast static site generator built for the modern web" />
</svelte:head>

<div class="min-h-screen bg-gradient-to-br from-neutral-900 via-black to-neutral-900 text-white">
	<section class="relative min-h-screen flex items-center">
		<div class="absolute inset-0 bg-gradient-to-br from-violet-600 via-violet-800/50 to-violet-500/10"></div>

		<div class="relative container mx-auto px-6 py-20">
			<div class="max-w-4xl mx-auto text-center">
				<div class="mb-8 {mounted ? 'animate-fade-in-up' : 'opacity-0'}">
					<div class="inline-flex items-center space-x-3 mb-6">
						<div class="w-12 h-12 bg-violet-300 rounded-lg flex items-center justify-center shadow-lg shadow-purple-600/25">
							<svg class="w-7 h-7 text-violet-900" fill="currentColor" viewBox="0 0 20 20">
								<path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/>
							</svg>
						</div>
						<h1 class="text-4xl md:text-5xl font-bold text-white">
							Amethyst
						</h1>
					</div>
				</div>

				<div class="mb-8 {mounted ? 'animate-fade-in-up delay-100' : 'opacity-0'}">
					<h2 class="text-5xl md:text-7xl font-bold mb-6 leading-tight">
						Build
						<span class="text-purple-400">
							Beautiful
						</span>
						<br />Static Sites
					</h2>
					<p class="text-xl md:text-2xl text-neutral-300 max-w-3xl mx-auto leading-relaxed">
						A modern static site generator that combines simplicity with power.
						Create lightning-fast websites with an elegant developer experience.
					</p>
				</div>

				<div class="cursor-pointer flex flex-col sm:flex-row gap-4 justify-center items-center mb-16 {mounted ? 'animate-fade-in-up delay-200' : 'opacity-0'}">
					<button on:click={() => window.open("https://github.com/CirklAI/amethyst/blob/main/README.md#installing", "_blank")} class="px-8 py-4 bg-gradient-to-r from-purple-600 to-purple-700 rounded-lg font-semibold text-lg text-white transition-all duration-300 hover:from-purple-700 hover:to-purple-800 -lg">
						Get Started
					</button>
					<button on:click={() => window.open("https://github.com/CirklAI/amethyst/blob/main/README.md#getting-started", "_blank")} class="cursor-pointer px-8 py-4 border-2 border-neutral-700 rounded-lg font-semibold text-lg transition-all duration-300 hover:border-purple-400 hover:text-purple-400">
						View Documentation
					</button>
				</div>
			</div>
		</div>
	</section>

	<section class="py-20 bg-neutral-950">
		<div class="container mx-auto px-6">
			<div class="max-w-6xl mx-auto">
				<h3 class="text-3xl md:text-4xl font-bold text-center mb-16 {mounted ? 'animate-fade-in' : 'opacity-0'}">
					Why Choose <span class="text-purple-400">Amethyst</span>?
				</h3>

				<div class="grid md:grid-cols-3 gap-8">
					<div class="p-8 rounded-lg bg-neutral-950 border-2 border-neutral-700 transition-all hover:border-purple-400 hover:shadow-lg hover:shadow-purple-400/20 {mounted ? 'animate-fade-in-up delay-300' : 'opacity-0'}">
						<div class="w-12 h-12 bg-gradient-to-br from-purple-600 to-purple-800 rounded-lg flex items-center justify-center mb-6 shadow-lg shadow-purple-600/25">
							<svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
								<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"/>
							</svg>
						</div>
						<h4 class="text-xl font-semibold mb-4 text-white">Lightning Fast</h4>
						<p class="text-neutral-300 leading-relaxed">
							Built for speed with optimized builds and minimal runtime overhead. Your sites load instantly.
						</p>
					</div>

					<div class="p-8 rounded-lg bg-neutral-950 border-2 border-neutral-700 transition-all hover:border-purple-400 hover:shadow-lg hover:shadow-purple-400/20 {mounted ? 'animate-fade-in-up delay-400' : 'opacity-0'}">
						<div class="w-12 h-12 bg-gradient-to-br from-purple-600 to-purple-800 rounded-lg flex items-center justify-center mb-6 shadow-lg shadow-purple-600/25">
							<svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
								<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10.325 4.317c.426-1.756 2.924-1.756 3.35 0a1.724 1.724 0 002.573 1.066c1.543-.94 3.31.826 2.37 2.37a1.724 1.724 0 001.065 2.572c1.756.426 1.756 2.924 0 3.35a1.724 1.724 0 00-1.066 2.573c.94 1.543-.826 3.31-2.37 2.37a1.724 1.724 0 00-2.572 1.065c-.426 1.756-2.924 1.756-3.35 0a1.724 1.724 0 00-2.573-1.066c-1.543.94-3.31-.826-2.37-2.37a1.724 1.724 0 00-1.065-2.572c-1.756-.426-1.756-2.924 0-3.35a1.724 1.724 0 001.066-2.573c-.94-1.543.826-3.31 2.37-2.37.996.608 2.296.07 2.572-1.065z"/>
								<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z"/>
							</svg>
						</div>
						<h4 class="text-xl font-semibold mb-4 text-white">Simple by design</h4>
						<p class="text-neutral-300 leading-relaxed">
							Quickly make a site in under 1 minute with a simple, intuitive tooling.<br>(yes, really!)
						</p>
					</div>

					<div class="p-8 rounded-lg bg-neutral-950 border-2 border-neutral-700 transition-all hover:border-purple-400 {mounted ? 'animate-fade-in-up delay-500' : 'opacity-0'}">
						<div class="w-12 h-12 bg-gradient-to-br from-purple-600 to-purple-800 rounded-lg flex items-center justify-center mb-6">
							<svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
								<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"/>
							</svg>
						</div>
						<h4 class="text-xl font-semibold mb-4 text-white">Simply Beautiful</h4>
						<p class="text-neutral-300 leading-relaxed">
							Clean architecture and thoughtful defaults. Build stunning sites without the complexity.
						</p>
					</div>
				</div>
			</div>
		</div>
	</section>

	<footer class="py-12 border-t-2 border-neutral-700 bg-neutral-900">
		<div class="container mx-auto px-6">
			<div class="flex flex-col md:flex-row justify-between items-center">
				<div class="flex items-center space-x-2 mb-4 md:mb-0">
					<div class="w-8 h-8 bg-gradient-to-br from-purple-600 to-purple-800 rounded-lg flex items-center justify-center -lg">
						<svg class="w-5 h-5 text-white" fill="currentColor" viewBox="0 0 20 20">
							<path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/>
						</svg>
					</div>
					<span class="font-semibold text-lg text-white">Amethyst</span>
				</div>
				<div class="text-neutral-400">
					© {new Date().getFullYear()} Cirkl Labs. Crafted with care.
				</div>
			</div>
		</div>
	</footer>
</div>

<style>
    @keyframes fade-in {
        from { opacity: 0; }
        to { opacity: 1; }
    }

    @keyframes fade-in-up {
        from {
            opacity: 0;
            transform: translateY(30px);
        }
        to {
            opacity: 1;
            transform: translateY(0);
        }
    }

    .animate-fade-in {
        animation: fade-in 0.4s ease-out forwards;
    }

    .animate-fade-in-up {
        animation: fade-in-up 0.4s ease-out forwards;
    }

    .delay-100 { animation-delay: 0.05s; }
    .delay-200 { animation-delay: 0.1s; }
    .delay-300 { animation-delay: 0.15s; }
    .delay-400 { animation-delay: 0.2s; }
    .delay-500 { animation-delay: 0.25s; }
</style>
