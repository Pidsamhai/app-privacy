<script lang="ts">
	import { page } from '$app/stores';
	import 'carbon-components-svelte/css/white.css';
	import '../app.css';
	import {
		Header,
		SkipToContent,
		Content,
		HeaderNav,
		HeaderNavItem
	} from 'carbon-components-svelte';
</script>

<Header company="PSM" platformName="App Privacy" href="/">
	<svelte:fragment slot="skip-to-content">
		<SkipToContent />
	</svelte:fragment>

	<HeaderNav>
		<HeaderNavItem href="/app/moviedb/privacy" text="Movie DB" isSelected={$page.url.pathname === "/app/moviedb/privacy"} />
	</HeaderNav>
</Header>

<Content>
	<slot />
</Content>
