<script lang="ts">
	import Card from '$lib/components/Card.svelte';
	import CardBody from '$lib/components/CardBody.svelte';
	import CardHead from '$lib/components/CardHead.svelte';
	import CardList from '$lib/components/CardList.svelte';
	import Container from '$lib/components/Container.svelte';

	let stuffs: ListItem[] = [
		{ name: 'Data Structures & Algorithms', link: 'https://github.com/ldriko/algorithms' },
		{ name: "Conway's Game of Life", link: 'https://conway.aldrico.live' }
	];
</script>

<Container>
	<div class="flex flex-col lg:flex-row gap-4">
		<div class="grow flex flex-col gap-4">
			<div class="flex flex-col sm:flex-row gap-4">
				<Card class="flex items-center justify-center">
					<img src="/heaven.webp" alt="Heaven" />
				</Card>
				<Card class="grow flex items-center justify-center">
					<CardBody>
						<h1 class="text-2xl lg:text-4xl">Hi! I'm Heaven</h1>
					</CardBody>
				</Card>
			</div>
			<Card>
				<CardHead>
					<h1 class="text-xl">About me:</h1>
				</CardHead>
				<CardBody>
					<ul class="list-disc mb-8 ms-4">
						<li>21 years old.</li>
						<li>Sophomore year Informatics student at UPN "Veteran" Jawa Timur.</li>
						<li>6 years of professional software engineering experience.</li>
					</ul>
					<ul class="list-disc ms-4">
						<li>
							Boring stuff: <a
								href="https://github.com/ldriko"
								class="text-blue-600 underline underline-offset-4"
							>
								GitHub
							</a>
							-
							<a
								href="https://linkedin.com/in/heaven-aldrico"
								class="text-blue-600 underline underline-offset-4"
							>
								Linkedin
							</a>
						</li>
						<li>
							Gamer: <a
								href="https://steamcommunity.com/id/ldriko/"
								class="text-blue-600 underline underline-offset-4"
							>
								Steam
							</a>
						</li>
						<li>
							Music: <a
								href="https://open.spotify.com/user/21ylwzfw5fbbg7hjoluerqeey"
								class="text-blue-600 underline underline-offset-4"
							>
								Spotify
							</a>
						</li>
					</ul>
				</CardBody>
			</Card>
		</div>
		<Card>
			<CardHead>
				<h1 class="text-xl">Some stuff you might not be interested in:</h1>
			</CardHead>
			<CardBody>
				<CardList items={stuffs} />
			</CardBody>
		</Card>
	</div>
	<div class="mt-[50%] text-center text-base italic">Yep. That's it.</div>
	<div class="mt-[250%] text-center text-base italic">Still nothing.</div>
	<div class="mt-[350%] text-center text-base italic">Won't stop won't you?</div>
	<div class="mt-[350%] text-center text-base italic">Are you that bored?</div>
	<div class="mt-[350%] text-center text-base italic">Okay.. you asked for it</div>
</Container>
