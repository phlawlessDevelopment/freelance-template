<script lang="ts">
	import { AppRail, AppRailAnchor } from '@skeletonlabs/skeleton';
	import { page } from '$app/stores';
	import Icon from '@iconify/svelte';
	import Footer from '../footer.svelte';
</script>

<AppRail>
	<svelte:fragment slot="lead">
		<AppRailAnchor href="/" selected={$page.url.pathname === '/'}>
			<div class="flex flex-col items-center justify-center">
				<Icon icon="mdi:home" class="h1" />
				<span>Home</span>
			</div>
		</AppRailAnchor>
	</svelte:fragment>
	<svelte:fragment slot="trail">
		<AppRailAnchor href="/login" selected={$page.url.pathname === '/login'}>
			<div class="flex flex-col items-center justify-center">
				<Icon icon="mdi:user" class="h1" />
				<span>Login</span>
			</div>
		</AppRailAnchor>
	</svelte:fragment>
</AppRail>
