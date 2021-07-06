<script>
    import Card from './Card.svelte'
</script>

<style>
    .container {
        width: 100%;
        display: flex;
        justify-content: center;
    }
    .container > div {
        width: calc(100% / 3);
    }
</style>

<div class="container">
    <div>
        <Card />
    </div>
</div>