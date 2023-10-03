<script lang="ts">
    import { page } from "$app/stores";
</script>


<div class="w-full h-[calc(100vh-10rem)] flex flex-col justify-center items-center">
    <h1>{$page.status}</h1>
    <hp>{$page.error?.message}</hp>
</div>
