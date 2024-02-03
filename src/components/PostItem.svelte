<script lang="ts">
    type Props={
        url:String,
        title:String,
    }
    import Date from "../components/Date.svelte";
    export let props:Props;
    const {url,title}=props;
</script>

<div class="my-6">
    <span class="text-xl font-semibold"><a href="/posts/{url}">{title}</a></span>
    <Date />
</div>

<style>
    a:hover{
        text-decoration: underline;
    }
    a{
        color: #0070f3;
    }
</style>