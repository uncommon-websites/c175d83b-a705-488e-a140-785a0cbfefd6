<script lang="ts">
    import Hero from '$lib/components/Hero.svelte';
    import SweetSpots from '$lib/components/SweetSpots.svelte';
    import FeaturesGrid from '$lib/components/FeaturesGrid.svelte';
    import ConnectDots from '$lib/components/ConnectDots.svelte';
    import FollowTeams from '$lib/components/FollowTeams.svelte';
    import DirectMessages from '$lib/components/DirectMessages.svelte';
    import Integrations from '$lib/components/Integrations.svelte';
    import FounderMemo from '$lib/components/FounderMemo.svelte';
    import Footer from '$lib/components/Footer.svelte';
</script>

<main class="bg-white min-h-screen">
    <Hero />
    <SweetSpots />
    <FeaturesGrid />
    <ConnectDots />
    <FollowTeams />
    <DirectMessages />
    <Integrations />
    <FounderMemo />
    <Footer />
</main>

