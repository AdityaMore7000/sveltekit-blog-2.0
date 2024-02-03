<script lang="ts">
    import Date from "../../../components/Date.svelte";
	import HomeLink from "../../../components/HomeLink.svelte";
import PostProfile from "../../../components/PostProfile.svelte";
</script>
<PostProfile/>

<section class="my-6 ">
    <h1 class="text-4xl font-extrabold">Two Forms of Pre-rendering</h1>
    <Date />
</section>

<article class="">
    <p>Next.js has two forms of pre-rendering: <strong>Static Generation</strong> and <strong>Server-side Rendering</strong>. The difference is in <strong>when</strong> it generates the HTML for a page.</p>
    <ul class="list-disc ml-8 my-4">
        <li><strong>Static Generation</strong> is the pre-rendering method that generates the HTML at <strong>build time</strong>. The pre-rendered HTML is then reused on each request.</li>
        <li><strong>Server-side Rendering</strong> is the pre-rendering method that generates the HTML on <strong>each request</strong>.</li>
    </ul>
    <p>Importantly, Next.js lets you <strong>choose</strong> which pre-rendering form to use for each page. You can create a "hybrid" Next.js app by using Static Generation for most pages and using Server-side Rendering for others.</p>

    <HomeLink />
</article>

<style>
    p,ul{
        font-size: 1.25rem;
    }
    p{
        margin-top: 1rem;
    }
</style>