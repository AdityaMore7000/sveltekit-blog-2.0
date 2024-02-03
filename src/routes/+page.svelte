<script>
	import PostItem from "../components/PostItem.svelte";
    const postList = [
        {
            url: "ssr-ssg",
            title: "When to Use Static Generation v.s. Server-side Rendering"
        },
        {
            url: "pre-rendering",
            title: "Two Forms of Pre-rendering"
        }
    ]
</script>
<section class="py-12 flex items-center flex-col gap-4">
        <img src = '/profile.jpeg' width="150" alt="Profile" class="rounded-full">
        <h1 class="text-5xl font-extrabold">Aditya More</h1>
</section>
<section class="text-2xl ">
    <h3>Hello, I'm <strong>Aditya</strong>, a pre-final year Student at PICT and a web developer. You can connect with me on <a class="hover:underline" target="_blank" href="https://www.linkedin.com/in/aditya-more-9a095422a/">LinkedIn</a></h3>
</section>
<section class="">
    <h2 class="text-3xl font-bold my-8">Blog</h2>
</section>
<section class="">
    {#each postList as post(post.title)}
        <PostItem props={post} />
    {/each}
</section>
<style>
    a{
        color: #0070f3;
    }
</style>