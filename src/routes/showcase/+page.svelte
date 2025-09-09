<script lang="ts">
	const items = [
		{
			image: '/image/showcase/slip2sure.png',
			url: 'https://slip2sure.com',
			title: 'Slip2Sure',
			description: 'บริการตรวจสอบสลิปโดยผ่านระบบ API'
		}
	];
</script>

<div class="container mx-auto">
	<div class="mt-6 grid grid-cols-3 gap-4">
		{#each items as item}
			<a href={item.url} aria-label={`Showcase ${item.title}, ${item.description} url.`}>
				<div
					class="group relative h-[400px] w-[600px] overflow-hidden shadow-md duration-300 hover:shadow-2xl rounded-md "
				>
					<img
						src={item.image || 'https://placehold.co/600x400/222/FFF'}
						alt={`Showcase ${item.title}, ${item.description}`}
						class="h-full w-full transform object-cover duration-300 group-hover:scale-105"
					/>

					<div
						class="absolute bottom-0 left-0 w-full translate-y-full bg-gradient-to-t from-black/70 to-transparent p-4 duration-300 group-hover:translate-y-0"
					>
						<h3 class="text-lg font-semibold text-white">{item.title}</h3>
						<p class="text-sm text-gray-200">
							{item.description}
						</p>
					</div>
				</div>
			</a>
		{/each}
	</div>
</div>
