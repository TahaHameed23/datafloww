<script>
	import logo from '$lib/assets/logo.svg';
	import DotBackground from '$lib/components/ui/DotBackground.svelte';
	import dashboard from '$lib/assets/dashboard.avif';
	import msfs from '$lib/assets/dataflow_ms.jpg';
	import AnimatedBeamMultipleInput from '$lib/components/ui/AnimatedBeamMultipleInput.svelte';
	import Card from '../lib/components/Card.svelte';
	import Social from '$lib/components/Social.svelte';
</script>

<div
	class="navbar-scroll navbar z-20 border-b border-gray-200 bg-slate-300 bg-opacity-40 backdrop-blur-lg backdrop-filter"
>
	<div class="navbar-start">
		<div class="dropdown">
			<div tabindex="0" role="button" class="btn btn-ghost lg:hidden">
				<svg
					xmlns="http://www.w3.org/2000/svg"
					class="h-5 w-5"
					fill="none"
					viewBox="0 0 24 24"
					stroke="currentColor"
				>
					<path
						stroke-linecap="round"
						stroke-linejoin="round"
						stroke-width="2"
						d="M4 6h16M4 12h8m-8 6h16"
					/>
				</svg>
			</div>
			<ul
				tabindex="-1"
				class="menu dropdown-content menu-sm z-[1] mt-3 w-52 rounded-box bg-white p-2 shadow"
			>
				<li class="text-lg"><a href="https://dash.datafloww.me/login">Login</a></li>
				<li class="text-lg"><a href="/">Home</a></li>
				<li class="text-lg"><a href="#features">Features</a></li>
			</ul>
		</div>
		<a href="https://datafloww.me">
			<img src={logo} alt="datafloww logo" class="mx-2" width="64" />
		</a>
		<p class="hidden px-2 text-xl font-bold lg:flex">Datafloww</p>
	</div>
	<div class="navbar-center hidden lg:flex">
		<ul class="menu menu-horizontal px-1">
			<li class="px-6 text-lg"><a href="/">Home</a></li>
			<li class="text-lg"><a href="#features">Features</a></li>
		</ul>
	</div>
	<div class="navbar-end">
		<a href="https://dash.datafloww.me/login">
			<button
				class="btn hidden bg-slate-100 lg:flex lg:rounded-full lg:border-x lg:border-y lg:border-blue-500 lg:px-7 lg:py-3 lg:text-blue-600 lg:hover:bg-slate-300"
			>
				Login
			</button>
		</a>
		<a href="https://dash.datafloww.me/signup">
			<button
				class="btn m-2 rounded-full border-none bg-blue-500 text-white hover:bg-blue-700 lg:mx-4"
			>
				Get started
			</button>
		</a>
	</div>
</div>

<div class="hero z-10">
	<DotBackground>
		<div class="hero-content animate-slidein300 text-center">
			<div class="max-w-2xl">
				<h1
					class="text-2xl font-semibold leading-tight md:text-3xl lg:text-4xl lg:font-bold lg:leading-snug"
				>
					Elevate your business <span
						class="bg-gradient-to-r from-[#3546ff] via-[#5aa6f8] to-blue-700 bg-clip-text text-transparent"
						>flow</span
					> with sharper analytics and product insights.
				</h1>
				<p
					class="text-md m-auto h-16 w-fit rounded-xl bg-slate-100 bg-opacity-80 px-1 py-5 font-medium lg:text-lg"
				>
					Unlock growth with data-driven decisions and actionable insights.
				</p>
				<a href="https://dash.datafloww.me">
					<button
						class="m-auto mt-10 w-fit animate-slidein500 cursor-pointer rounded-full bg-blue-500 p-3 text-lg text-white duration-300 hover:px-4 hover:shadow-xl hover:shadow-blue-400 hover:duration-300 md:p-3 md:text-sm lg:mt-2 lg:text-base"
						>Get Started
					</button>
				</a>
			</div>
		</div>
	</DotBackground>
</div>

<div
	class="relative h-40 w-full animate-slidein700 overflow-hidden bg-slate-50 md:h-[22rem] lg:h-[30.4rem]"
>
	<img src={dashboard} alt="" class="px-3 lg:px-28" />
</div>
<div class=" overflow-hidden bg-slate-100 pt-20">
	<h1 class="text-center text-2xl font-semibold lg:text-5xl">
		Get every <span
			class="bg-gradient-to-r from-[rgb(53,70,255)] via-[#5aa6f8] to-blue-700 bg-clip-text text-transparent"
			>insight</span
		> at one place!
	</h1>
	<AnimatedBeamMultipleInput />
</div>

<div class="py-8 bg-dot-black/[0.4]">
	<h1 class="mb-6 text-center text-3xl font-semibold lg:text-4xl" id="features">Features</h1>
	<div class="grid w-full grid-cols-1 gap-y-8 lg:grid-cols-2">
		<Card />
	</div>
</div>

<div
	class="mb-5 flex w-full justify-center bg-gradient-to-b from-slate-50 to-slate-100 px-5 py-10 lg:px-44 lg:py-20"
>
	<img src={msfs} class="drop-shadow-lg" alt="" />
</div>

<div class="grid grid-cols-4 border-2 border-t-gray-300 bg-slate-100 text-center text-lg">
	<Social />
</div>
