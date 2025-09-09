<script lang="ts">
	const items = [
		{
			url: 'https://github.com/mrwan2546/tools',
			title: 'tools',
			description: 'The web-tool for any generate. It\'s simple but powerful 🔥'
		},
		{
			url: 'https://github.com/mrwan2546/promptparse-py',
			title: 'promptparse-go',
			description: 'All-in-one Python for PromptPay & EMVCo QR Codes'
		},
		{
			url: 'https://github.com/mrwan2546/promptparse-go',
			title: 'promptparse-go',
			description: 'All-in-one Golang for PromptPay & EMVCo QR Codes'
		}
	];
</script>

<div class="container mx-auto">
	<div class="mt-6 grid grid-cols-3 gap-4">
		{#each items as item}
			<a
				href={item.url}
				aria-label={`Showcase ${item.title}, ${item.description} url.`}
				class="bg-white/5 p-5 flex flex-row gap-3 rounded-md scale-100 hover:scale-[1.03] duration-300 drop-shadow-none hover:drop-shadow-md drop-shadow-white"
			>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 24 24"
					fill="none"
					stroke="currentColor"
					stroke-width="2"
					stroke-linecap="round"
					stroke-linejoin="round"
					class="w-[32px] text-white"
				>
					<line x1="6" x2="6" y1="3" y2="15" /><circle cx="18" cy="6" r="3" /><circle
						cx="6"
						cy="18"
						r="3"
					/>
					<path d="M18 9a9 9 0 0 1-9 9" />
				</svg>
				<div class="text-white">
					<h1 class="font-bold text-xl">{item.title}</h1>
					<p class="text-sm">{item.description || 'nil'}</p>
				</div>
			</a>
		{/each}
	</div>
</div>
